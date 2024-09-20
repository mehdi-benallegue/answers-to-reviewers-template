# Response to Reviewers LaTeX Template

A comprehensive LaTeX template for preparing responses to reviewers' comments during the peer-review process. This template provides structured environments for quoting reviewer comments, referencing parts of your manuscript, and citing external sources. It also includes annotation commands for tracking revisions and changes.

## Features

- **Structured Response Format**: Easily organize your responses with custom environments.
- **Reviewer Comments**: Use the `revquote` environment to include reviewer comments in shaded boxes.
- **Manuscript Quotes**: Quote excerpts from your manuscript using the `quotepaper` environment.
- **External Quotes**: Use the `externalquote` environment to include quotes from external sources with optional author attribution.
- **Annotations**: Custom commands for highlighting important notes and tracking pending changes.

## Getting Started

To use this template, clone the repository and include the provided LaTeX file in your project. You can customize the appearance by adjusting the color definitions and environment settings in the preamble.

### Prerequisites

- LaTeX distribution (e.g., TeX Live, MikTeX)
- Compatible LaTeX editor (e.g., Overleaf, TeXShop, Texmaker)

### Compilation

The template is designed to be compiled using `pdflatex`. This ensures that all features, including custom fonts and special characters, are properly supported.

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/[your-username]/response-to-reviewers-template.git
   ```

2. Navigate to the directory:
   ```bash
   cd response-to-reviewers-template
   ```

3. Open the `response-template.tex` file in your preferred LaTeX editor.

4. Compile the document using `pdflatex`:
   ```bash
   pdflatex response-template.tex
   ```

## Usage

### Including Reviewer Comments

Use the `revquote` environment to include reviewer comments in shaded boxes:

```latex
\begin{revquote}
[Insert reviewer comment here.]
\end{revquote}
```

### Quoting Excerpts from Your Manuscript

Use the `quotepaper` environment to quote excerpts from your own paper, either the old or revised version:

```latex
\begin{quotepaper}
[Insert excerpt from your paper here.]
\end{quotepaper}
```

### Including External Quotes

Use the `externalquote` environment to include quotes from external sources with optional alignment and author attribution:

```latex
\begin{externalquote}[c]{Author Name}
[Insert external quote here.]
\end{externalquote}
```

### Adding Annotations

Use the provided custom commands to add annotations and alerts within your document:

- Highlight important notes or alerts:
  ```latex
  \alert{This is an important note.}
  ```

- Insert a reminder to verify section or reference numbers:
  ```latex
  As mentioned in Section~\qo\ref{sec:method}, we have updated the algorithm.
  ```

- Indicate a promised change that has not yet been implemented:
  ```latex
  We will update the figure in the next revision.\io
  ```

## Customization

You can customize the appearance of the template by modifying the color definitions and environment settings in the preamble. For example, to change the background color of the `revquote` environment, adjust the `colback` parameter in its definition.

## License

This project is licensed under the BSD 3-Clause License - see the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue for any suggestions or improvements.

## Acknowledgments

This template was developed by Mehdi Benallegue at the CNRS AIST Joint Robotics Laboratory to help researchers streamline the peer-review response process.
