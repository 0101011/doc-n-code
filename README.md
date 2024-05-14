## 10 Fast Rules for Documenting Software

1. **Write Comments as You Code**
   - Comments are crucial for understanding code later
   - Write comments as you code to capture your thought process
   - Aim for a balanced amount of comments, not too few or too many

```python
# Bad (no comments)
for sequence in parsed_sequences: 
    analyze(sequence)

# Bad (too many comments)  
# iterate over the genes in the genome
for sequence in parsed_sequences:
    # call the analyze function, passing it each gene as argument
    analyze(sequence) 

# Good (just enough)
# Analyze the genome 
for sequence in parsed_sequences:
    analyze(sequence)
```

2. **Include Examples (and Lots of Them)**
   - Examples provide a starting point for experimentation
   - Include examples demonstrating key functionality  
   - Examples can also serve as unit tests

3. **Include a Quickstart Guide**
   - Help users get started with your software quickly
   - Use examples, tutorials, videos, or other formats
   - Test your quickstart guide to ensure it's effective

4. **Include a README File with Basic Information**
   - The README acts as the homepage for your project
   - Include installation, configuration, documentation links, license, testing, and acknowledgments
   - Consider using badges to show project status

5. **Include a Help Command for Command Line Interfaces**
   - Document how to use your CLI with a "help" command
   - Include usage, subcommands, options/arguments, environment variables, and examples
   - Use tools like click (Python) to generate the help command

6. **Version Control Your Documentation**  
   - Keep documentation in your version control repository
   - Archive rendered documentation for each release
   - Provide a changelog to track changes between versions

7. **Fully Document Your Application Programming Interface (API)** 
   - Document inputs, outputs, errors, methods, and attributes
   - Follow a consistent style guide for API documentation

8. **Use Automated Documentation Tools**
   - Tools like Sphinx, Doxygen, and MkDocs can generate documentation
   - Automate API documentation, interactive REST API docs, and more
   - Use services like Read the Docs to keep documentation up-to-date  

9. **Write Error Messages that Provide Solutions or Point to Documentation**
   - Good error messages state the error, software state, and how to fix it
   - Provide guidance in error messages to save users' time

```python
# Bad
print("Error: Translation failed.")

# Good  
print("Error: Translation failed because of an invalid codon (\"IQT\") "
      "in position 1 in sequence 41. Ensure this is a valid DNA "
      "sequence and not a protein sequence.")
```

10. **Tell People How to Cite Your Software**
    - Include DOI, BibTeX entry, and written reference in the README
    - Use a CITATION file in Citation File Format (CFF)
    - Get a DOI for your software from services like Zenodo or JOSS

## Additional Tips

- **Use Consistent Formatting**
    - Use a consistent style for headers, code blocks, etc.
    - Markdown allows for consistent formatting across platforms

```markdown
### Header 3

#### Header 4

`inline code`

```python
# Code block
print("Hello World!")
```

- **Structure Documentation Well**
    - Break documentation into logical sections and chapters
    - Use tables of contents and cross-references where appropriate

- **Include Visual Aids**
    - Use diagrams, flowcharts, and screenshots to clarify concepts
    - Reference images using relative paths

- **Make Documentation Searchable**
    - Use proper headings and anchor links
    - Consider using a search plugin for websites

- **Keep Documentation Up-to-Date**
    - Automate documentation updates when code changes
    - Encourage contributors to update documentation
