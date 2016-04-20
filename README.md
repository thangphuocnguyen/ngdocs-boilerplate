
A small custom from https://github.com/Quramy/generator-ngdoc to support render ngdocs for Angular Project

## Setup:

 1. clone ngdocs-boilerplate into your directory
 2. `$ cd docs`
 3. `$ npm install`
 4. `$ bower install`
 5. In **docs/gulp/dgeni.js**, add your source path into readFilesProcessor.sourceFiles for document generate references
   
 # Ex:

      `readFilesProcessor.sourceFiles = [
          {
            include: '../samplesrc/app/**/*.js',
            basePath: 'samplesrc'
          }
        ];`

 6. Generate your ngdocs documents, init docs server by:
      `$ gulp docs:serve:dist`
    
 
 # Note: **
    
 For clean previous build assets:

    `$ gulp docs:clean`

## Gulp Tasks:

+ Generate ngdoc and run document application on Node.js server.
    `$ gulp docs:serve`

+ Build document application package, and place in directory 'docs/dist'.
    `$ gulp docs:build`

+ Run document application package created by docs:build task on Node.js web server.
    `$ gulp docs:serve:dist`

+ Clean previous build assets:
    `$ gulp docs:clean`


## Ngdocs syntax references:

+ dgeni tags support: https://github.com/angular/angular.js/wiki/Writing-AngularJS-Documentation
+ angular document styles: https://github.com/angular/angular.js/tree/master/src
+ ngdoc guideline: https://github.com/idanush/ngdocs/wiki/API-Docs-Syntax
+ Notes from dgeni: https://github.com/angular/dgeni-packages/blob/master/NOTES.md

