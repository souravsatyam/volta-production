** Clone the existing repo **

git clone https://github.com/souravsatyam/volta-production.git

** Copy the content of cloned repo in empty express project


** Modify routes of index routes of empty express project

  ```  var express = require('express');
    var router = express.Router();
    var path = require('path');
    var appDir = path.dirname(require.main.filename);


    /* GET home page. */
        router.get('/*', function(req, res, next) {

        res.sendFile(path.join(appDir, '/public/', 'index.html'));

        });  

    module.exports = router; ```


    