# AngularQuizApp

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 12.2.11.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## if you are facing Error: error:0308010C:digital envelope routines::unsupported
    
    at new Hash (node:internal/crypto/hash:68:19)
    at Object.createHash (node:crypto:138:10)
    at BulkUpdateDecorator.hashFactory (D:\angular\Quiz Game\node_modules\webpack\lib\util\createHash.js:145:18)
    at BulkUpdateDecorator.update (D:\angular\Quiz Game\node_modules\webpack\lib\util\createHash.js:46:50)
    at RawSource.updateHash (D:\angular\Quiz Game\node_modules\webpack\node_modules\webpack-sources\lib\RawSource.js:77:8)
    at NormalModule._initBuildHash (D:\angular\Quiz Game\node_modules\webpack\lib\NormalModule.js:880:17)
    at handleParseResult (D:\angular\Quiz Game\node_modules\webpack\lib\NormalModule.js:946:10)
    at D:\angular\Quiz Game\node_modules\webpack\lib\NormalModule.js:1040:4
    at processResult (D:\angular\Quiz Game\node_modules\webpack\lib\NormalModule.js:755:11)
    at D:\angular\Quiz Game\node_modules\webpack\lib\NormalModule.js:819:5 {
  opensslErrorStack: [ 'error:03000086:digital envelope routines::initialization error' ],
  library: 'digital envelope routines',
  reason: 'unsupported',
  code: 'ERR_OSSL_EVP_UNSUPPORTED'
}

Node.js v20.11.0
then make it like
On Unix-like (Linux, macOS, Git bash, etc.):

export NODE_OPTIONS=--openssl-legacy-provider
On Windows command prompt:

set NODE_OPTIONS=--openssl-legacy-provider
On PowerShell:

$env:NODE_OPTIONS = "--openssl-legacy-provider"

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
