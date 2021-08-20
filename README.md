## README

#### Setup

- npx create-react-app leafletdemo
- npm install leaflet
- npm install react-leaflet

#### Error

- Error message

```
./node_modules/@react-leaflet/core/esm/path.js 10:41
Module parse failed: Unexpected token (10:41)
File was processed with these loaders:

./node_modules/babel-loader/lib/index.js
  You may need an additional loader to handle the result of these loaders.
  | useEffect(function updatePathOptions() {
  | if (props.pathOptions !== optionsRef.current) {

  >       const options = props.pathOptions ?? {};
  >
  > | element.instance.setStyle(options);
  > | optionsRef.current = options;

```

#### Solution

- change package.json file

```
"browserslist": [
">0.2%",
"not dead",
"not op_mini all"
]

```

- remove .cache directory from node_module/ directory

```

```
