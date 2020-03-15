# Typography Chart 


| **Scale Category** | **Typeface** | **Font**  | **Size**  |   **Case**  | **Line Height** | **Word Spacing** | **Letter Spacing** |
| ------------------ | ------       | -----     | -----     |     -----   |  -----          | -----            | -----              |
| XXL                | Open Sans    | Regular   | 42px-48px |Title Case   | 1.5             | .16em            | .12em              |
| XL                 | Open Sans    | Regular   | 34px-42px |Title Case   | 1.5             | .16em            | .12em              |
| L                  | Open Sans    | Semibold  | 28px-34px |Title Case   | 1.5             | .16em            | .12em              |
| M                  | Open Sans    | Semibold  | 22px-28px |Title Case   | 1.5             | .16em            | .12em              |
| S                  | Open Sans    | Semibold  | 18px-24px |Title Case   | 1.5             | .16em            | .12em              |
| XS                 | Open Sans    | Regular   | 16px-22px |Sentence Case| 1.5             | .16em            | .12em              |
| Body, Input        | Open Sans    | Semibold  | 16px      |Sentence Case| 1.5             | .16em            | .12em              |
| Labels             | Open Sans    | Regular   | 16px      |Title Case   | 1.5             | .16em            | .12em              |
| Label Caption/Help | Open Sans    | Regular   | 14px      |Sentence Case| 1.5             | .16em            | .12em              |
| Button             | Open Sans    | Bold      | 19px      |Title Case   | 1.5             | .16em            | .12em              |



# The Code

**The Calculation**

h1 {

  font-size: calc([minimum size] + ([maximum size] - [minimum size]) * ((100vw - [minimum viewport width]) / ([maximum viewport width] - [minimum viewport width])));
  
  }

<br>

**Example**

html {

	font-size: 100%;
	line-height: 1.5 !important;
	word-spacing: 0.16em !important;
	letter-spacing: 0.12em !important;
}

<br>

h1 {

	font-size: calc(42px + (48 - 42) * ((100vw - 320px) / (1200 - 320)));
}

# More About This Method
* https://css-tricks.com/snippets/css/fluid-typography/