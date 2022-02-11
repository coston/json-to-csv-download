# ⌗ json-to-csv-export

A function to easily generate csv downloads of your json data. ✨

[![npm package version](https://badge.fury.io/js/json-to-csv-export.svg)](https://www.npmjs.com/package/json-to-csv-export)&nbsp;
[![npm downloads](https://img.shields.io/npm/dm/json-to-csv-export.svg)](https://www.npmjs.com/package/json-to-csv-export)&nbsp;
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://prettier.io)

## Live Demo

[https://json-to-csv-export.coston.io](https://json-to-csv-export.coston.io)

## Features

- Create a csv/json download from data
- Convert json/csv data
- Lightweight
- Easy to use
- optional filename

## Install

Install with npm:

```sh
npm i json-to-csv-export
```

Or load from a CDN:

```html
<script src="https://cdn.jsdelivr.net/npm/json-to-csv-export"></script>
```

## Example Usage

```html
import csvDownload, { jsonDownload, jsonToCsv, csvToJson } from 'json-to-csv-export'

...

  <button onClick={() => csvDownload(jsonData)}>
    Download CSV Data
  </button>
...

  <code>
    {jsonToCsv(jsonData).data}
  </code>

...
  <button onClick={() => jsonDownload(csvData)}>
    Download JSON Data
  </button>

...

  <code>
    {csvToJson(csvData).data}
  </code>
```

### Download Arguments
| #   | Argument  | Type     | Requirement | Default      | Description                       |
| --- | --------- | -------- | ----------- | ------------ | --------------------------        |
| 1   | data      | `object` | `required`  | `null`       | string or object                  |
| 2   | filename  | `string` | `optional`  | "export.[csv\|json]" | The complete filename     |
| 3   | delimiter | `string` | `optional`  | ","          | field separator                   |

### Converter Arguments
| #   | Argument  | Type     | Requirement | Default      | Description                       |
| --- | --------- | -------- | ----------- | ------------ | --------------------------        |
| 1   | data      | `object` | `required`  | `null`       | string or object                  |
| 2   | delimiter | `string` | `optional`  | ","          | field separator                   |

### Callable Functions
#### `csvDownload()`
Singular function to convert and download JSON to CSV data. This is shown in an example above.

#### `jsonDownload()`
Singular function to convert and download CSV to JSON data. This is shown in an example above.

#### `csvToJson()`
Convert CSV data into JSON data.
<details>
  <summary>Returns</summary>
  <br/>
  <pre font-size="1" p="3" bg="lightgray" class="prism-code css-108ro8y">
    { data:string, error:string }
  </pre>
</details>

#### `jsonToCsv()`
Convert JSON data into CSV data.
<details>
  <summary>Returns</summary>
  <br/>
  <pre font-size="1" p="3" bg="lightgray" class="prism-code css-108ro8y">
    { data:string, error:string }
  </pre>
</details>

## Contributing

Please help provide good data faster! Submit any issues and/or make a pull request!