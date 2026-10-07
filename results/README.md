# Test results

Every implementation from this list that can be built and run on Linux, tested with the same black-box cases by [json2dir-tester](https://github.com/json2dir-guru/json2dir-tester). The cases are this list's [conformance suite](../conformance/README.md), cases collected from other implementations' own test suites, and a security set: nothing may be written outside the target directory. Each implementation is built from its own repository with its own toolchain, and the resulting directory tree is compared with the expected one.

<div id="results" data-src="results.json">
  <p>The interactive table needs JavaScript. The raw data is in <a href="results.json">results.json</a>.</p>
</div>

<script src="results.js" defer></script>

## Updating

The page renders [`results.json`](results.json) and nothing else, so replacing that file is the whole update. The tester writes it from a test campaign:

```sh
json2dir-tester export --dir <campaign directory> --out <directory>
cp <directory>/results.json results/results.json
```
