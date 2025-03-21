#  ؜JavaScript ھەققىدە چۈشەنچە

  بىز JavaScript نىڭ ئالاھىدىلىكىنى، ئۇنىڭ بىلەن نېمىلەرنى ئەمەلگە ئاشۇرالايدىغانلىقىمىزنى ۋە باشقا قايسى تېخنىكىلار بىلەن ئۇنى ياخشى «ئوينايدىغانلىقىمىز»نى كۆرۈپ باقايلى.

  ## ؜JavaScript دېگەن نېمە؟

  ؜*JavaScript* دەسلەپتە «تور بەتلەرنى جانلاندۇرۇش» ئۈچۈن قۇرۇلغان.

  بۇ تىلدىكى پىروگراممىلار *scripts* دەپ ئاتىلىدۇ. ئۇلار تور بەتنىڭ HTML ئىچىدە يېزىلىپ، بەت يۈكلەنگەندە ئاپتوماتىك ئىجرا بولالايدۇ.

  ؜`Script` لار ئادەتتىكى تېكىست يېزىق شەكلىدە تەمىنلىنىدۇ ۋە ئىجرا قىلىنىدۇ. ئۇلار ئىجرا بولۇش ئۈچۈن ئالاھىدە مۇھىت تەييارلىقى ياكى ئالدىن «تەرجىمە» قىلىشقا موھتاج ئەمەس.

  بۇ جەھەتتە JavaScript بولسا[Java](https://en.wikipedia.org/wiki/Java_programming_language)بىلەن ئىنتايىن پەرقلىنىدۇ

  

  > ؜JavaScript قۇرۇلغاندا دەسلەپكى قەدەمدە يەنە بىر ئىسمى بار ئىدى: `LiveScript` . لېكىن ئەينى ۋاقىتتا Java ناھايىتى ئالقىشقا ئېرىشكەن، شۇڭا يېڭى بىر تىلنى Java نىڭ «كىچىك ئىنىسى» قىلىپ بېكىتىشنى قارار قىلىنغان.
  >
  > ئەمما ئۇنىڭ تەرەققىي قىلىشىغا ئەگىشىپ JavaScript ئۆزىنىڭ خاسلىقى [ECMAScript](http://en.wikipedia.org/wiki/ECMAScript) دەپ ئاتىلىدىغان تولۇق مۇستەقىل تىلغا ئايلاندى، ھازىر ئۇنىڭ Java بىلەن ئازراقمۇ مۇناسىۋىتى يوق.

  

  بۈگۈنكى كۈندە JavaScript تور كۆرگۈچتىلا ئەمەس، بەلكى مۇلازىمىتېردىمۇ ئىجرا بولالايدۇ، ياكى ئەمەلىيەتتە [JavaScript موتورى](https://en.wikipedia.org/wiki/JavaScript_engine) دەپ ئاتىلىدىغان ئالاھىدە پىروگرامما بار ھەرقانداق ئۈسكۈنىدە ئىجرا بولالايدۇ.

  تور كۆرگۈچتە «JavaScript مەۋھۇم ماشىنىسى» دەپ ئاتىلىدىغان بىر خىل قىستۇرما ھالەتتىكى گىرەلەشتۈرۋەتكەن موتور بار.

  ئوخشىمىغان ماتورلارنىڭ ئوخشىمىغان «كود نامى» بار. مەسىلەن:

  - بىرىنچى : Chrome, Opera ياكى Edge دا – [V8](https://en.wikipedia.org/wiki/V8_JavaScript_engine)
  - ئىككىنچى: Firefox دا – [SpiderMonkey](https://en.wikipedia.org/wiki/SpiderMonkey)
  - يەنە IE ئۈچۈن "چاكرا"، سافارى ( Safari ) ئۈچۈن "JavaScriptCore", "Nitro" ياكى "SquirrelFish" دېگەندەك .

  يۇقىرىقى ئاتالغۇلارنى ئەستە ساقلاش ئاسان، چۈنكى توردىكى ئاچقۇچىلار يېتەكچى ماتېرىياللىرىدا كۆپ ئىشلىتىلىدۇ. بىزمۇ ئۇلارنى ئىشلىتىمىز. مەسىلەن، ئەگەر «بىر ئىقتىدار X نى V8 قوللىغان» بولسا، بەلكىم Chrome، Opera ۋە Edge دا ئىشلىشى مۇمكىن.

  

  > موتور مۇرەككەپ. ئەمما ئاساسىي ئىشلار ئاسان.
  >
  > 1. موتور (ئەگەر تور كۆرگۈچ بولسا ئاللىبۇرۇن تەييار) ئاۋۋال Script نى ئوقۇپ يېشىدۇ.
  > 2. ئاندىن موتور ئۇنى ماشىنا كودىغا ئايلاندۇرىدۇ (تەرجىمە قىلىدۇ).
  > 3. ئاندىن ماشىنا كودى خېلى تىز سۈرئەتتە ئىجرا بولىدۇ.
  >
  > موتور بۇ جەرياننىڭ ھەر بىر قەدىمىدە ئەلالاشتۇرۇش ئىلىپ بارىدۇ. ئۇ ھەتتا ماشىنا كودىغا تەرجىمە قىلىنغان Script ئىجرا بولۇش جەريانىدا كۆزىتىش ئىلىپ بېرىپ، ئۇنىڭدا ئىشلەتكەن سانلىق مەلۇماتلارنى تەھلىل قىلىپ، ھەم شۇ بىلىملەرگە ئاساسەن ماشىنا كودىنى يەنىمۇ ئەلالاشتۇرىدۇ.

  

  

  ## ئۇنداقتا تور كۆرگۈچتىكى JavaScript نېمىلەرنى قىلالايدۇ ؟

  ھازىرقى زامان JavaScript بولسا «بىخەتەر» پىروگرامما تىلى. ئىچكى ساقلىغۇچ ياكى CPU غا تۆۋەن (يەنى ئاساسى) قاتلاملىق بۇيرۇق بىلەن كىرىشنى تەمىنلىمەيدۇ، چۈنكى بۇ تىل دەسلەپتە شۇنى تەلەپ قىلمايدىغان تور كۆرگۈچلەر ئۈچۈن قۇرۇلغان.

  يەنە JavaScript نىڭ ئىقتىدارى ئۇ ئىجرا بولۇۋاتقان مۇھىتقا زور دەرىجىدە باغلىق بولىدۇ. مەسىلەن: [Node.js](https://wikipedia.org/wiki/Node.js) بولسا JavaScript نىڭ ئۆز ئالدىغا ھۆججەتلەرنى ئوقۇش/يېزىش، تور تەلىپىنى بىرتەرەپ قىلىش قاتارلىق ئىقتىدارلارنى قوللايدۇ.

  تور كۆرگۈچتىكى JavaScript بولسا ئىشلەتكۈچى ياكى تور مۇلازىمىتېر بىلەن ئۇچۇر ئالماشتۇرۇش دېگەندەك توربەتكە مۇناسىۋەتلىك ھەرقانداق مەشغۇلاتنى ئىلىپ بارالايدۇ.

  

  مەسىلەن، تور كۆرگۈچ ئىچىدىكى JavaScript مۇنۇ مەشغۇلاتلارغا پۇختا:

  - بەتكە يېڭى HTML قوشۇش، بار بولغان مەزمۇننى ئۆزگەرتىش، ئۇسلۇبلارنى ئۆزگەرتىش.
  - ئىشلەتكۈچىنىڭ ھەرىكىتىگە ئىنكاس قايتۇرۇش، مائۇس چېكىلگەندە ئىجرا بولۇش، مائۇس يۆتكەلگەندە ياكى كۇنۇپكا بېسىلغاندىكى مەشغۇلات.
  - تور ئارقىلىق يىراقتىكى مۇلازىمىتېرلارغا تەلەپ يوللاش، ھۆججەتلەرنى چۈشۈرۈش ۋە يۈكلەش (ئاتالمىش [AJAX](https://en.wikipedia.org/wiki/Ajax_(پىروگرامما)) ۋە [COMET](https://en.wikipedia.org/wiki/Comet_(پىروگرامما)) تېخنىكىلىرى).
  - كوكىي (Cookie) نى ئېلىش ۋە بېكىتىش، زىيارەتچىگە سوئال قويۇش، ئۇچۇر كۆرسىتىش.
  - زىيارەت قىلغۇچى (Client) تەرەپتىكى سانلىق مەلۇماتلارنى ئەستە تۇتۇش ("يەرلىكتە ساقلاش").

  

  ## يەنە ئۇنداقتا تور كۆرگۈچتىكى JavaScript نېمىلەرنى قىلالمايدۇ ؟

  شۇنداق، JavaScript نىڭ تور كۆرگۈچتىكى ئىقتىدارى ئابۇنتلارنىڭ بىخەتەرلىكىنى قوغداش بىلەنلا چەكلىنىدۇ. مەقسەت: بىر رەزىل تور بەتنىڭ شەخسىي ئۇچۇرغا ئېرىشىش ياكى ئىشلەتكۈچىنىڭ سانلىق مەلۇماتىغا زىيان يەتكۈزۈشىنىڭ ئالدىنى ئېلىش.

  بۇنداق چەكلىمىلەرنىڭ مىساللىرى تۆۋەندىكىلەرنى ئۆز ئىچىگە ئالىدۇ:

  

  - بىر تور بەتتىكى JavaScript قاتتىق دىسكىدا خالىغانچە ھۆججەتلەرنى ئوقۇمايدۇ/ يازمايدۇ، كۆچۈرۈپ چاپلىمايدۇ ياكى پىروگراممىلارنى ئىجرا قىلمايدۇ. ئۇنىڭ OS (مەشغۇلات سىستېمىسى) ئىقتىدارىغا بىۋاسىتە كىرىش ئىجازىتى يوق.

    ھازىرقى زامان تور كۆرگۈچلەر ھۆججەتلەرنى ئىشلىتىشكە يول قويىدۇ، ئەمما زىيارەت قىلىش چەكلىك ھەم پەقەت ئىشلەتكۈچى مەلۇم مەشغۇلاتلارنى قىلغاندىلا ئاندىن بۇ ئىقتىدارنى تەمىنلەيدۇ، مەسىلەن، ھۆججەتنى تور كۆرگۈچ كۆزنىكىگە «تاشلاش» ياكى `<input>` خەتكۈش ئارقىلىق تاللاش دېگەندەك.

    كامېرا/مىكروفون قاتارلىق ئۈسكۈنىلەر بىلەن ئالاقە قىلىش ئۇسۇللىرى بار، ئەمما ئۇلار ئىشلەتكۈچىنىڭ ئېنىق بولغان رۇخسىتىنى تەلەپ قىلىدۇ. شۇڭا JavaScript نى قوللايدىغان بەت تور كامېراسىنى ئوغرىلىقچە قوزغاپ، ئەتراپنى كۆزەتمەيدۇ ۋەياكى ئۇچۇرنى [NSA](https://en.wikipedia.org/wiki/National_Security_Agency) غا يوللىمايدۇ.

  - ئوخشاش بولمىغان  tabs/windows ئادەتتە بىر-بىرىنى بىلمەيدۇ. ئەمما بەزىدە شۇنداق قىلىدۇ، مەسىلەن بىر كۆزنەك JavaScript ئارقىلىق يەنە بىر كۆزنەكنى ئاچقاندا. ئەمما بۇ ئەھۋالدىمۇ يەنە بىر بەتتىكى مەزمۇن ئوخشاش بولمىغان تور بېكەتلەردىن (ئوخشىمىغان ئادرېس، دائىرە، كېلىشىم ياكى پورتتىن) كەلگەن بولسا ئۇنداقتا مۇشۇ بەتنى ئاچقاندىكى JavaScript مۇ ئۇ بەتنىڭ مەزمۇنىغا ئېرىشمەيدۇ

    بۇ «ئوخشاش مەنبە سىياسىتى» (Same Origin Policy) دەپ ئاتىلىدۇ. باشقا بېكەتنىڭ ياكى بەتنىڭ ئۇچۇرىغا ئېرىشىش ئۈچۈن *ھەر ئىككى تور بەت (ياكى بېكەت)* ئۆز-ئارا سانلىق مەلۇمات ئالماشتۇرۇشقا قوشۇلۇشى، چوقۇم ئۇنى بىر تەرەپ قىلىدىغان ئالاھىدە JavaScript كودى بولۇشى كېرەك. بىز بۇنى دەرسلىكتە سۆزلەيمىز.

    بۇ چەكلىمە، يەنە شۇ ئىشلەتكۈچىنىڭ بىخەتەرلىكى ئۈچۈن. ئابۇنت ئاچقان (http://anysite.com) تور بېكەت كۆزنىكى ئادرېسى (http://gmail.com) بولغان يەنە بىر كۆزنەكتىكى ئۇچۇرغا ئېرىشىشكە ئامالسىز ھەم بۇنداق قىلىشقا بولمايدۇ، مەسىلەن، ئۇ تور بېكەتتىن ئۇچۇر ئوغرىلىسا بولمايدۇ.

  - شۇنداقلا JavaScript نۆۋەتتىكى بېكەتنىڭ مۇلازىمىتېرى بىلەن تور ئارقىلىق ئاسانلا ئالاقە قىلالايدۇ. ئەمما ئۇنىڭ باشقا (باشقا كۆزنەكتىكى) تور بېكەت/دائىرلەردىن سانلىق مەلۇمات قوبۇل قىلىش ئىقتىدارى بولمايدۇ. مۇمكىن بولسىمۇ، مۇلازىمىتېردىن ئېنىق كېلىشىم (HTTP بەت بېشى ئۇچۇرىدا ئىپادىلەنگەن) تەلەپ قىلىدۇ. يەنە بىر قېتىم تەكىتلىسەك، بۇ بىخەتەرلىكنى كۆزدە تۇتقان چەكلىمە خالاس.

  ![](limitations.svg)

  ئەمما JavaScript نى تور كۆرگۈچنىڭ سىرتىدا ئىشلىتىلسە بۇنداق چەكلىمىلەر مەۋجۇت ئەمەس، مەسىلەن بىر مۇلازىمىتېردا. زامانىۋى تور كۆرگۈچلەرمۇ قىستۇرمىلارنىڭ ھەرخىل ئىجازەتلەرنى تەلەپ قىلىشقا يول قويىدۇ.

  ## ؜JavaScript نى ئۆزگىچە قىلغان زادى نېمە؟

  بۇيەردە JavaScript نى مۇشۇنداق «يامان» قىلالىغان ئاز دېگەندە *3* چوڭ ئىش بار:

  > + ؜HTML/CSS لار بىلەن تولۇق ئىچ قۇيۇن، تاش قۇيۇن بولۇپ كېتىش.
  > + ئاددىي ئىشلارنى ئاددىي بىرتەرەپ قىلىش.
  > + بارلىق چوڭ تور كۆرگۈچلەرنى قوللايدۇ ۋە سۈكۈتتىكى ھالەتتىلا قوللايدۇ.

  

  مانا بۇ JavaScript بۇ *ئۈچ چوڭ ئىشنى* بىرلەشتۈرگەن بىردىنبىر تور كۆرگۈچ تېخنىكىسى.

  مانا بۇ JavaScript نى ئۆزگىچە قىلىدۇ. دەل مۇشۇ سەۋەبتىن تور كۆرگۈچ كۆرۈنمە يۈزىنى قۇرۇشتا ئەڭ كەڭ دائىرىدە ئىشلىتىلىدىغان قورال ھېسابلىنىدۇ.

  دېمەكچى، JavaScript ئارقىلىق مۇلازىمىتېر، كۆچمە ئەپ قاتارلىقلارنى قۇرغىلى بولىدۇ.

  ## ؜JavaScript نىڭ ئەتراپىدا «ئوينايدىغان» تىللار

  بىرىنچى، JavaScript نىڭ سىنتاكسىسلىق نۇسخىسى (Syntax) ھەممە ئادەمنىڭ ئېھتىياجىغا ماس كەلمەيدۇ. ئوخشىمىغان كىشىلەر ئوخشاش بولمىغان ئالاھىدىلىككە ئېرىشىشنى ئۈمىد قىلىدۇ.

  مۇشۇنداق بولۇشى كېرەك، چۈنكى ئوخشىمىغان كىشىلەرنىڭ تۈرلىرى ھەم تەلىپى ئوخشىمايدۇ.

  شۇڭا، يېقىندا تور كۆرگۈچتە ئىجرا بولۇشتىن بۇرۇن JavaScript قا ئۆزگەرتىلىدىغان (تەرجىمە قىلىنىدىغان) بىر تۈركۈم يېڭى تىللار پەيدا بولدى.

  ھازىرقى زامان قوراللىرى تەرجىمە قىلىشنى ئىنتايىن تېز ھەم ئېنىق قىلىدۇ، شۇڭا ئاچقۇچىلارنىڭ باشقا بىر تىلدا كود يېزىشىغا ۋە «يەڭنىڭ ئاستىدا ئاپتوماتىك ئايلاندۇرۇش»غا (بىلىندۈرمەي تەرجىمە قىلىدۇ دېمەكچى) يول قويىدۇ.

  مۇشۇنداق تىللاردىن مىساللار:

  - بىرىنچىسى [CoffeScript](https://coffeescript.org) بولسا JavaScript نىڭ «سىنتاكسىك شېكەر تېلى » (Syntactic Sugar) دەپ ئاتىلىدۇ. قىسقىراق سىنتاكسىسنى ئىشلىتىپ، تېخىمۇ ئوچۇق، تېخىمۇ ئېنىق كود يېزىشىمىزغا يول قويىدۇ. ئادەتتە Ruby چىلار مۇشۇنى ياخشى كۆرىدۇ.
  - ئىككىنچىسى [TypeScript](https://www.typescriptlang.org) بولسا «قاتتىق تۈزۈم ئاستىدا سانلىق مەلۇمات يېزىش»نى (Strict Data Typing) ئاددىيلاشتۇرۇشنى مەركەز قىلىپ، مۇرەككەپ تۈزۈلمىلەرنى قوللىشىنى ھەم تۈر ئىچىشنى بىرقەدەر ئاددىيلاشتۇرىدۇ. بۇنى مىكروسوفت تەتقىق قىلىپ چىققان.
  - ئۈچىنچىسى [Flow](https://flow.org/) يەنە شۇ (Data Typing) قىلىدىغان، ئەمما باشقىچە ئۇسۇلدا قىلىدىغان تىل. فەيسبۇك شىركىتى تەتقىق قىلىپ ياسىغان.
  - تۆتىنچىسى [Dart](https://www.dartlang.org/) تور كۆرگۈچسىز مۇھىتتا ماڭىدىغان (كۆچمە ئەپكە ئوخشاش)، ئۆز ئالدىغا مۇستەقىل موتورغا ئىگە بىر تىل، شۇنداقلا JavaScript قا بىرلەشتۈرۈپ ئىشلەتكىلى بولىدۇ. گۇگۇل شىركىتى تەتقىق قىلىپ ياسىغان.
  - بەشىنچىسى [Brython](https://brython.info/)بولسا Python نىڭكىنى JavaScript قا ئايلاندۇرغۇچ بولۇپ، JavaScript ئىشلەتمەيلا ساپ Python دا قوللىنىشچان پىروگراممىلارنى يېزىشنى قوللايدۇ.
  - ئاخىرقىسى [Kotlin](https://kotlinlang.org/docs/reference/js-overview.html)بولسا تور كۆرگۈچ ياكى Node نى نىشانلىغان زامانىۋى، ئىخچام ۋە بىخەتەر پىروگرامما تىلى.

  يۇقارقىلىرى بىلەنلا چەكلەنمەيدۇ. ئەلۋەتتە، بۇ تەرجىمە قىلىدىغان تىللارنىڭ بىرىنى ئىشلەتسەكمۇ، ئەمما يەنىلا JavaScript نى ھەقىقىي چۈشىنىپ بېقىشىمىز كېرەك.

  ## خۇلاسە

  - ئەڭ دەسلەپتە JavaScript تور كۆرگۈچكە ماس كېلىدىغان تىل سۈپىتىدە بارلىققا كەلگەن، ئەمما ھازىر باشقا نۇرغۇن مۇھىتتىمۇ ئىشلىتىلىۋاتىدۇ.
  - بۈگۈنكى كۈندە JavaScript ھەم HTML/CSS بىلەن تولۇق بىرلەشتۈرۈلگەن ئەڭ كەڭ قوللانغان تور كۆرگۈچ تىلى بولۇش سۈپىتى بىلەن ئۆزگىچە ئورۇنغا ئىگە.
  - يەنەJavaScript قا «تەرجىمە» قىلىدىغان ۋە مەلۇم ئىقتىدارلارنى تەمىنلەيدىغان نۇرغۇن تىللار بار. JavaScript نى پىششىق ئىگىلىگەندىن كېيىن، ھېچ بولمىغاندا ئۇلارغا بىر قاراپ قويۇشنى تەۋسىيە قىلىمىز.
