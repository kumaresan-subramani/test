{
    "env": {
        "browser": true,
        "es2021": true
    },
    "extends": [
        "eslint:recommended",
        "plugin:@typescript-eslint/recommended",
        "plugin:jsdoc/recommended"
    ],
    "parser": "@typescript-eslint/parser",
    "parserOptions": {
        "ecmaFeatures": { "js": true },
        "ecmaVersion": 2018,
        "project": "./tsconfig.json",
        "sourceType": "module"
      },
    "plugins": [
        "@typescript-eslint",
        "@typescript-eslint/tslint",
        "jsdoc"
    ],
    "rules": {
        "use-isnan": "error",
        "@typescript-eslint/tslint/config": [
            "error",
            {
                "rules": {
                    "ban": true,
                    "chai-vague-errors": true,
                    "max-func-body-length": [
                        true,
                        120,
                        {
                            "ignore-parameters-to-function-regex": "describe"
                        }
                    ],
                    "missing-jsdoc": true,
                    "no-backbone-get-set-outside-model": false,
                    "no-cookies": false,
                    "no-delete-expression": false,
                    "no-disable-auto-sanitization": true,
                    "no-duplicate-case": true,
                    "no-duplicate-parameter-names": true,
                    "no-empty-interfaces": false,
                    "no-exec-script": true,
                    "no-function-expression": false,
                    "no-multiple-var-decl": false,
                    "no-string-based-set-immediate": false,
                    "no-string-based-set-interval": false,
                    "no-unnecessary-bind": false,
                    "no-unused-imports": true,
                    "no-with-statement": false,
                    "prefer-array-literal": false,
                    "typedef": [
                        true,
                        "call-signature",
                        "parameter",
                        "property-declaration",
                        "variable-declaration",
                        "arrow-parameter",
                        "member-variable-declaration"
                    ],
                    "use-named-parameter": false,
                    "valid-typeof": true,
                    "whitespace": [
                        true,
                        "check-branch",
                        "check-decl",
                        "check-operator",
                        "check-separator",
                        "check-type"
                    ]
                }
            }
        ],
        "no-control-regex": "error",
        "no-constant-condition": "error",
        "no-invalid-regexp": "error",
        "curly": "error",
        "eol-last": [
            "error",
            "always"
        ],
        "guard-for-in": "error",
        "no-labels": "error",
        "max-len": [
            "error",
            {
                "code": 140,
                "tabWidth": 4,
                "ignoreComments": true,
                "ignoreStrings": true,
                "ignoreTemplateLiterals": true,
                "ignoreRegExpLiterals": true
            }
        ],
        "no-console": [
            "error",
            {
                "allow": [
                    "warn",
                    "dir",
                    "timeLog",
                    "assert",
                    "clear",
                    "count",
                    "countReset",
                    "group",
                    "groupEnd",
                    "table",
                    "dirxml",
                    "error",
                    "groupCollapsed",
                    "Console",
                    "profile",
                    "profileEnd",
                    "timeStamp",
                    "context"
                ]
            }
        ],
        "no-redeclare": [
            "error",
            {
                "builtinGlobals": true
            }
        ],
        "@typescript-eslint/no-parameter-properties": "error",
        "@typescript-eslint/indent": [
            "error",
            4,
            {
                "CallExpression": {
                    "arguments": "first"
                },
                "FunctionDeclaration": {
                    "parameters": "first"
                },
                "FunctionExpression": {
                    "parameters": "first"
                }
            }
        ],
        "no-debugger": "error",
        "no-eval": "error",
        "no-extra-semi": "error",
        "no-throw-literal": "error",
        "no-fallthrough": "error",
        "comma-dangle": [
            "error",
            "never"
        ],
        "no-trailing-spaces": "error",
        "@typescript-eslint/no-unused-expressions": "error",
        "@typescript-eslint/no-var-requires": "error",
        "one-var": [
            "error",
            "always"
        ],
        "@typescript-eslint/no-explicit-any": "error",
        "no-cond-assign": [
            "error",
            "always"
        ],
        "@typescript-eslint/consistent-type-assertions": "off",
        "jsdoc/check-alignment": "error",
        "no-empty": "error",
        "quotes": [
            "error",
            "single"
        ],
        "semi": [
            "error",
            "always"
        ],
        "eqeqeq": [
            "error",
            "smart"
        ],
        "valid-typeof": [
            "error",
            {
                "requireStringLiterals": true
            }
        ],
        "camelcase": [
            "error",
            {
                "properties": "always",
                "ignoreDestructuring": true,
                "ignoreImports": true
            }
        ],
        "no-irregular-whitespace": [
            "error",
            {
                "skipStrings": true,
                "skipComments": true,
                "skipRegExps": true,
                "skipTemplates": true
            }
        ],
        "valid-jsdoc": [
            "error",
            {
                "prefer": {
                    "arg": "param",
                    "argument": "param",
                    "class": "constructor",
                    "return": "returns",
                    "virtual": "abstract"
                }
            }
        ],
        "no-var": "error",
        "radix": "error"
    },
    "reportUnusedDisableDirectives": true,
    "overrides": [
        {
            "files": [
                "node_modules",
                "dist",
                "public",
                "coverage",
                "test-report"
            ],
            "rules": {
                "no-unused-expressions": "off"
            }
        }
    ]
}
