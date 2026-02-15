# merge-pdf


This is a Jupyter notebook that, given a folder of `.docx` files, merge them into a single `.pdf` file.

The resulting file has bookmarks (one for each input docx file), and can have an overlay with (1) page numbers (2) text (e.g. "Working papers - please do not cite") (3) date of creation.

Useful to put together an academic paper from multiple docx (title page, paper, tables, figures).

## Usage

In the folder of docx files, create a JSON file following this template:

```
{
    "files_map": {
        "main.pdf": [
			"title_page.docx",
			"research_highlights.docx",
            "paper.docx",
            "table_1.docx",
            "table_2.docx",
            "figure_1.docx",
			"figure_2.docx",
			"figure_3.docx",
        ],
        "blackhole": [
			"credit_statement.docx"
        ],
		"appendix.pdf": [
			"appendix.docx",
		    "table_S1a.docx",
			"table_S1b.docx",
		]
    },
    "overlay": {
		"overlay": true,
		"font_size": 9,
		"font_family": "my_aptos",
		"font_file": "C:/data/software/Microsoft Aptos Fonts/Aptos.ttf",
		"snapshot_date": false,
		"page_number": true,
		"working_paper": false
	}
}
```

`blackhole` is a special placeholder: files listed there are not converted into an PDF.

`docx` files not mapped in any `files_map` throw an exception.
