# TSConfig Policy

## Official Recommendation Policy

* Sets the following compiler options because it's recommended in [Intro to the TSConfig Reference](https://www.typescriptlang.org/tsconfig):
  * alwaysStrict: true
  * esModuleInterop: true
  * exactOptionalPropertyTypes: true
  * forceConsistentCasingInFileNames: true
  * noImplicitAny: true
  * noImplicitThis: true
  * skipLibCheck: true
  * strict: true
  * strictBindCallApply: true
  * strictFunctionTypes: true
  * strictNullChecks: true
  * strictPropertyInitialization: true

## Language and Environment Policy

* Sets the following compiler options because many frameworks/libraries use decorators:
  * experimentalDecorators: true

## Emit Policy

* Sets the following compiler options for providing runtime information:
  * declaration: true
  * declarationMap: true
  * sourceMap: true
* Sets the following compiler options for reducing code size:
  * removeComments: true

## JavaScript Support Policy

* Sets the following compiler options for JavaScript support:
  * allowJs: true
  * checkJs: true