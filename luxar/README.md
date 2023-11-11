# Luxar v7.9.5 - CopyRight©

  # How-to use Patcher
    const luxar = require('luxar');
    luxar.patcher("https://URL.HERE/");

  # How-to use RandomUUID
    const luxar = require('luxar');
    luxar.RandomUUID(Length);

  # How-to use Mailer
    const luxar = require('luxar');
    const data= {
      from: "your email",
      to: "to mail",
      subject: "your subject",
      text: "your text", 
    };
    const user= {
      service: "use service",
      user: "your email",
      pass: "your pass",
    };
    luxar.Mailer(data,user);

  # How-to use Wardon
    const luxar = require('luxar');
    const err ={
      filename: "err filename.log",
      level: "err level \ default 2",
    };
    luxar.Wardon("your message","level / default 4",err,"your filename.log \ default combined.log");

  # How-to use SmartStorage
    const luxar = require('luxar');

    luxar.SmartStorage.set('name', 'John');
    console.log(luxar.SmartStorage.get('name'));
    luxar.SmartStorage.remove('name');
    console.log(luxar.SmartStorage.get('name')); 

  # How-to use NoteMe
    const luxar = require('luxar');
    const config ={
      title: "your title",
      message: "your message",
      wait: "true \ false",
      icon: "iconPath",
      sound: "oggFilePath.ogg",
    };

    luxar.NoteMe(config);

  # How-to use cellBackAPI
    const luxar = require('luxar');
    luxar.cellBackAPI("endpoint \ example api/point", "method", "your data", "https://yourURL.com");

  # How-to use WebServiceClient
    const luxar = require('luxar');
    const webService = new luxar.WebServiceClient('https://api.yourURL.com');

      # toGet
      webService.get('/endpoint')
        .then(data => {
          console.log('data:', data);
        })
        .catch(error => {
          console.error('ErrorOrder:', error);
        });

      # toPost
      const dataToPost = { email: 'example@gmail.com', password: e0x0a0m0p0l0e1 };
      webService.post('/endpoint', dataToPost)
        .then(data => {
          console.log('Done post !', data);
        })
        .catch(error => {
          console.error('ErrorOrder:', error);
        });

  # How-to use MathOperations
    const luxar = require('luxar');
    console.log(luxar.MathOperations.add(5, 3)); // print 8
    console.log(luxar.MathOperations.subtract(10, 4)); // print 6
    console.log(luxar.MathOperations.multiply(7, 2)); // print 14
    console.log(luxar.MathOperations.divide(8, 2)); // print 4


  # How-to use RandomCode
    const luxar = require('luxar');
    luxar.RandomCode(10); // started at 8 to 10000

  # How-to use zArchive
    const luxar = require('luxar');

    # To Compress
    luxar.zArchive.compressFile('filename.type', 'compressFilename.zip');

    # To Decompress
    luxar.zArchive.decompressFile('compressFilename.zip', 'filename.type');

  # How-to use AnalyzeText
    const luxar = require('luxar');
    const sampleText = "Compromise is a natural language processing library for Node.js.";
    const analysisResult = luxar.AnalyzeText(sampleText);

    console.log('Sentences:', analysisResult.sentences);
    console.log('Terms:', analysisResult.terms);
    console.log('Entities:', analysisResult.entities);

  # How-to use MuRcPerformance
    const luxar = require('luxar');
      function timeConsumingOperation() {
        let result = 0;
        for (let i = 0; i < 1000000; i++) {
          result += i;
        }
        console.log('Operation Result:', result);
    };

    luxar.MuRcPerformance(() => {
      timeConsumingOperation();
    });





