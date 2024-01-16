
def pytest_generate_tests(metafunc):
    # Read the data from the markdown file
    filename = metafunc.config.getoption("--datafile")
    with open(filename, "r") as f:
        data = f.read()

    # Split the data into headers, subheaders, paragraphs, and code snippets
    headers, subheaders, paragraphs, code_snippets = split_data(data)

    # Generate test functions for each code snippet
    for i, (header, subheader, paragraph, code) in enumerate(zip(headers, subheaders, paragraphs, code_snippets)):
        metafunc.parametrize(
            "header, subheader, paragraph, code",
            [(header, subheader, paragraph, code)],
        )