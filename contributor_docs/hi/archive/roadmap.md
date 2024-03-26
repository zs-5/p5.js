# p5.js 1.0 रोडमैप [WIP]

यह दस्तावेज़ भविष्य के 1.0 संस्करण p5.js. के लिए संभावित सुविधाओं, सुधारों और रखरखाव मदों की एक सूची है। पहला मसौदा कार्य समूह द्वारा यूसीएलए डिजाइन मीडिया आर्ट्स में बनाया गया था और आपकी प्रतिक्रिया के लिए बाहर रखा गया है। यह एक कामकाजी मसौदा है जिसे अद्यतन किया जा सकता है और इसे अगस्त 2019 के लिए p5.js योगदानकर्ता सम्मेलन में संशोधित किया जाएगा। हमारा लक्ष्य 2019 के अंत तक p5.js 1.0 जारी करना है।

ईएस 6 प्रवास के अपवाद के साथ, यहां कार्यों को प्राथमिकता से आदेश नहीं दिया गया है। गथुब पर [मील के पत्थर](https://github.com/processing/p5.js/milestones) है, जहां हम रिलीज और ट्रैक प्रगति के लिए कार्यों को प्राथमिकता देते हैं।

## ES6 प्रवास
* चरण 1: उपयोगकर्ता का सामना करना पड़ रहा है
  * p5js.org ट्यूटोरियल (प्रति ट्यूटोरियल इश्यू)
  * p5js.org उदाहरण (प्रति अनुभाग समस्या)
  * p5js.org संदर्भ उदाहरण (प्रति अनुभाग जारी)
* चरण 2: डेवलपर का सामना करना पड़ रहा है
  * प्रक्रियाओं का निर्माण
  * डेवलपर
* चरण 3: कोडबेस
  * टीबीडी: यह एक समर्पित व्यक्ति द्वारा किया जा सकता है, हम इस पर शुरू नहीं करेंगे जब तक कि यह निर्धारित न हो।
* बाद का चरण:
  * अन्य सामग्री - किस हद तक बाहरी सामग्री (p5.js पुस्तक के साथ शुरू करना, कोडिंग ट्रेन) को शैक्षिक संसाधनों के एक चिकनी रोलआउट को सुनिश्चित करने के लिए अद्यतन करने की आवश्यकता है?
  * योगदान पुस्तकालयों

## रखरखाव
* लंबित क्रोम परिवर्तनों के लिए ऑडियो अपडेट (उपयोगकर्ता को पहले बातचीत करनी चाहिए)
  * अद्यतन संदर्भ प्रलेखन और उदाहरण, और उदाहरण पृष्ठ
  * इस बारे में चेतावनी देने के लिए FES अपडेट करें?
* अधिक पूर्ण इकाई परीक्षण
  * ऐसा करने के लिए स्पष्ट ट्यूटोरियल
* मित्रतापूर्ण त्रुटि प्रणाली प्रलेखन में सुधार
  * इस प्रक्रिया में क्या हो रहा है, इसे बेहतर दस्तावेज़ के लिए टिप्पणियों को https://github.com/processing/p5.js/blob/main/src/core/friendly_errors/fes_core.js पर जोड़ें।

## बग फिक्सिंग
* मोबाइल डिवाइस का समर्थन / उन्नयन
* WebGL मजबूती
  * प्रकाश
    * रोशनी () कार्यान्वयन
    * डिफ़ॉल्ट रूप से प्रति पिक्सेल प्रकाश व्यवस्था
    * शेडर पाइपलाइन को सरल बनाएं?
    * अद्यतन उदाहरण
  * आकार पाइपलाइन को सरल बनाएं
    * आकृतियों के लिए एक रेंडरिंग विधि, रिटेन मोड से जियोम ऑब्जेक्ट का निर्माण करें

## नए विशेषताएँ
* आकृतियाँ
  * createShape () p5.Geometry ऑब्जेक्ट वापस करने के लिए सार्वजनिक API ?? 2D में समतुल्य क्या है?
  * 2 डी के लिए एसवीजी कुछ भी?
* छवि के साथ GIF समर्थन ()
  * createImg एक अच्छा काम है लेकिन छात्रों को gifs पसंद है :)
* I18n (स्थानीयकरण) त्रुटि संदेशों के लिए + FES
  * स्थानीय त्रुटि के लिए बुनियादी ढांचे का विकास करना और कोडबेस के भीतर संदेशों को सांत्वना देना
  * विभिन्न त्रुटि संदेशों का अनुवाद करें
* K-12 समर्थन के रूप में चर्चा की [धागे में](https://github.com/processing/p5.js/issues/2305)
  * सर्कल () और वर्ग जोड़ें ()
  * पुस्तकालयों पृष्ठ पर makeyourownalgorithmicart / simple.js प्राप्त करें
* पुस्तकालय भर में वादों को लागू करें
  * कोडबेस में प्रोमिस के उपयोग की पुष्टि / कार्यान्वयन
  * लोड एक्सएक्सएक्स (लोड प्राथमिकता) के लिए एपीआई में प्रोमिस का खुला उपयोग?
  
## योगदानकर्ता प्रक्रिया और समर्थन
* विभिन्न क्षेत्रों में अपूर्णता के लिए खुले टिकट:
  * परिक्षण
  * फ़ीचर कार्यान्वयन
  * अनुवाद
* [शब्दार्थ संस्करण](https://semver.org/) का कठोर उपयोग
* भविष्य के संस्करणों के लिए रोडमैप इनपुट को सुलझाने के लिए स्पष्ट प्रक्रिया।

## आदि
* 1.0 रिलीज के लिए, कलाकारों और कोडर से क्यूरेटेड उदाहरणों का एक नया सेट ड्रॉप करें।