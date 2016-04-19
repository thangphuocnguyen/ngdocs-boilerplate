Install:

 1. clone ngdocs-boilerplate into your directory
 2. `cd docs`
 3. `$ npm install`
 4. `$ bower install`
 5. In **docs/gulp/dgeni.js**, add your source path into readFilesProcessor.sourceFiles for document generate references
   
   Ex:
   

      readFilesProcessor.sourceFiles = [
          {
            include: '../samplesrc/app/**/*.js',
            basePath: 'samplesrc'
          }
        ];

 6. Generate your ngdocs documents, init docs server by:
   
   

      $ gulp docs:serve:dist
    
 
  ** Note **
    
 For clean previous build assets:

    $ gulp docs:clean
