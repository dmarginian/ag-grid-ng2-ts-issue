- Run 'npm install'
- Note the failure, it appears tsc is trying to compile main.ts in node_modules/ag-grid-ng2.
- Modify src/tsconfig.json, remove the following line - "rootDir": "./",
- Run 'npm install'
- Examine the dist directory, note the compiled js is underneath 'src'
- Remove node_modules/ag-grid-ng2/main.ts
- Run 'npm install' again
- Examine the dist directory, note the compiled js is directly underneath dist (where is should be)