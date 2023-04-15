## Links

### .editorconfig

1. [EditorConfig](https://editorconfig.org/)
2. [EditorConfig Specification¶](https://spec.editorconfig.org/)
3. [.prettierrc.json + .editorconfig](https://prettier.io/docs/en/configuration.html)
4. [max_line_length issue - deprecate?](https://github.com/editorconfig/editorconfig/issues/387)

```md
# Stop the editor from looking for .editorconfig files in the parent directories

# root = true

[*]

# Non-configurable Prettier behaviors

charset = utf-8
insert_final_newline = true

# Caveat: Prettier won’t trim trailing whitespace inside template strings, but your editor might.

# trim_trailing_whitespace = true

# Configurable Prettier behaviors

# (change these if your Prettier config differs)

end_of_line = lf
indent_style = space
indent_size = 2
max_line_length = 100

[*.js]
max_line_length = 120

[*.md]
max_line_length = 200
```

### husky and lint-staged

1. https://prettier.io/docs/en/precommit.html
   - `npx mrm@2 lint-staged`
2. https://github.com/typicode/husky
3. [lint-staged](https://github.com/okonet/lint-staged)

## Prettier

1. https://prettier.io/

```json
{
  "arrowParens": "always",
  "bracketSameLine": true,
  "bracketSpacing": false,
  "embeddedLanguageFormatting": "auto",
  "htmlWhitespaceSensitivity": "css",
  "insertPragma": false,
  "jsxSingleQuote": true,
  "singleAttributePerLine": false,
  "printWidth": 300,
  "proseWrap": "preserve",
  "quoteProps": "as-needed",
  "requirePragma": false,
  "semi": true,
  "singleQuote": true,
  "tabWidth": 2,
  "trailingComma": "es5",
  "useTabs": false,
  "vueIndentScriptAndStyle": false,
  "endOfLine": "auto"
}
```

## Eslint

1. https://eslint.org/
2. [Configure ESLint](https://eslint.org/docs/latest/use/configure/)
3. https://eslint.org/docs/latest/rules/array-element-newline
   ```json
    "array-element-newline": ["error", {
    "ArrayExpression": "consistent",
    "ArrayPattern": { "minItems": 3 },
    }]
   ```
4. eslint-plugin-import/docs/rules [import/order](https://github.com/import-js/eslint-plugin-import/blob/main/docs/rules/order.md)
   ```json
   {
     "import/order": [
       "error",
       {
         "pathGroups": [
           {
             "pattern": "react",
             "group": "builtin",
             "position": "before"
           }
         ],
         "pathGroupsExcludedImportTypes": ["react"]
       }
     ]
   }
   ```

### eslint-plugin-prettier

- [eslint-plugin-prettier](https://github.com/prettier/eslint-plugin-prettier)

### eslint-plugin-html

1. [eslint-plugin-html](https://github.com/BenoitZugmeyer/eslint-plugin-html)

### stylelint.io

- https://stylelint.io/user-guide/get-started/

## Introduction guides

1. [These tools will help you write clean code](https://www.freecodecamp.org/news/these-tools-will-help-you-write-clean-code-da4b5401f68e)
   - [ru-translate](https://habr.com/ru/company/ruvds/blog/428173/)
2. [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)
3. [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html)
