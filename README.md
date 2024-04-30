# EgoFormer: Ego-Gesture Classification in Context of Autonomous Driving <br/>
 Link to paper: [![Paper](https://img.shields.io/badge/paper-IEEE%20Sensors-blue)](https://ieeexplore.ieee.org/document/10508297)

## Abstract <br/>
<p align="justify"> Decoding the intentions of passengers and other road users remains a critical challenge for autonomous vehicles and intelligent transportation systems. Hand gestures are key in these interactions, offering a direct communication channel. Moreover, egocentric videos mimic a first-person perspective, aligning closely with human visual perception. Yet, the development of deep learning algorithms for detecting egocentric hand gestures in autonomous driving is hindered by the absence of useful datasets. Furthermore, there is a pressing need for gesture recognition methods to evolve from CNN-based architectures to transformer models. To address these challenges, we present EgoDriving, a novel dataset of egocentric hand gestures, curated for driving-related hand gestures. Finally, we introduce EgoFormer, an efficient video transformer for egocentric hand gesture classification that is optimized for edge computing deployments. EgoFormer incorporates a Video Dynamic Position Bias (VDPB) module to enhance long-range positional awareness and leverage absolute positions from convolutional sub-layers within its transformer blocks. Designed for low-resource settings, EgoFormer offers substantial reductions in inference latency and GPU utilization while maintaining competitive accuracy against state-of-the-art hand gesture recognition frameworks.</p>

## EgoDriving Dataset
<p align="center">
<img src = "images/Qazi3_Hand_gestures.jpg " alt="Raw image" width="50%"/>
</p>

## Overall pipeline
<p align="center">
<img src = "images/Egoformer_pipeline.png " alt="Raw image" width="50%" align="center"/>
</p>

## VDPB
<p align="center">
<img src = "images/VDPB.png " alt="Raw image" width="50%" align="center"/>
</p>

## Performance comparison on EgoDriving dataset
<table id="tabular">
<tbody>
<tr style="border-top: none !important; border-bottom: none !important;">
<td style="text-align: center; border-left-style: solid !important; border-left-width: 1px !important; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top-style: solid !important; border-top-width: 1px !important; width: auto; vertical-align: middle; ">Method</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top-style: solid !important; border-top-width: 1px !important; width: auto; vertical-align: middle; ">Top-1</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top-style: solid !important; border-top-width: 1px !important; width: auto; vertical-align: middle; ">F1 Score</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top-style: solid !important; border-top-width: 1px !important; width: auto; vertical-align: middle; ">Precision</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top-style: solid !important; border-top-width: 1px !important; width: auto; vertical-align: middle; ">Recall</td>
</tr>
<tr style="border-top: none !important; border-bottom: none !important;">
<td style="text-align: center; border-left-style: solid !important; border-left-width: 1px !important; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; ">Video Transformer Models</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; " class="_empty"></td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; " class="_empty"></td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; " class="_empty"></td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; " class="_empty"></td>
</tr>
<tr style="border-top: none !important; border-bottom: none !important;">
<td style="text-align: center; border-left-style: solid !important; border-left-width: 1px !important; border-right-style: solid !important; border-right-width: 1px !important; border-bottom: none !important; border-top: none !important; width: auto; vertical-align: middle; ">TimeSformer [20]</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom: none !important; border-top: none !important; width: auto; vertical-align: middle; ">57.81</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom: none !important; border-top: none !important; width: auto; vertical-align: middle; ">-</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom: none !important; border-top: none !important; width: auto; vertical-align: middle; ">-</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom: none !important; border-top: none !important; width: auto; vertical-align: middle; ">-</td>
</tr>
<tr style="border-top: none !important; border-bottom: none !important;">
<td style="text-align: center; border-left-style: solid !important; border-left-width: 1px !important; border-right-style: solid !important; border-right-width: 1px !important; border-bottom: none !important; border-top: none !important; width: auto; vertical-align: middle; ">MotionFormer [19]</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom: none !important; border-top: none !important; width: auto; vertical-align: middle; ">-</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom: none !important; border-top: none !important; width: auto; vertical-align: middle; ">-</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom: none !important; border-top: none !important; width: auto; vertical-align: middle; ">-</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom: none !important; border-top: none !important; width: auto; vertical-align: middle; ">-</td>
</tr>
<tr style="border-top: none !important; border-bottom: none !important;">
<td style="text-align: center; border-left-style: solid !important; border-left-width: 1px !important; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; ">VideoSwin [36]</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; ">-</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; ">-</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; ">-</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; ">-</td>
</tr>
<tr style="border-top: none !important; border-bottom: none !important;">
<td style="text-align: left; border-left-style: solid !important; border-left-width: 1px !important; border-right-style: solid !important; border-right-width: 1px !important; border-bottom: none !important; border-top: none !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; " colspan="5">Hand Gesture Classification Models</td>
</tr>
<tr style="border-top: none !important; border-bottom: none !important;">
<td style="text-align: center; border-left-style: solid !important; border-left-width: 1px !important; border-right-style: solid !important; border-right-width: 1px !important; border-bottom: none !important; border-top: none !important; width: auto; vertical-align: middle; ">RGDC [30]</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom: none !important; border-top: none !important; width: auto; vertical-align: middle; ">10.00</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom: none !important; border-top: none !important; width: auto; vertical-align: middle; ">9.195</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom: none !important; border-top: none !important; width: auto; vertical-align: middle; ">10.057</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom: none !important; border-top: none !important; width: auto; vertical-align: middle; ">9.195</td>
</tr>
<tr style="border-top: none !important; border-bottom: none !important;">
<td style="text-align: center; border-left-style: solid !important; border-left-width: 1px !important; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; ">TBNDR [23]</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; ">36.67</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; ">34.02</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; ">36.72</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; ">36.67</td>
</tr>
<tr style="border-top: none !important; border-bottom: none !important;">
<td style="text-align: center; border-left-style: solid !important; border-left-width: 1px !important; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; ">EgoFormer(Ours)</td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; "><span class="math-inline ">
<mjx-container class="MathJax" jax="SVG"><svg style="vertical-align: -0.025ex" xmlns="http://www.w3.org/2000/svg" width="6.302ex" height="1.554ex" role="img" focusable="false" viewBox="0 -676 2785.7 687"><g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)"><g data-mml-node="math"><g data-mml-node="TeXAtom" data-mjx-texclass="ORD"><g data-mml-node="mn"><path data-c="36" d="M48 318Q48 395 68 456T120 553T193 613T273 646T350 655Q425 655 461 616T497 524Q497 485 475 468T428 451Q399 451 378 470T357 521Q357 565 403 588Q375 601 351 601Q313 601 282 584Q242 565 222 526Q199 473 199 367Q201 369 210 380T227 396T246 410T275 422T312 426Q438 426 494 332Q526 285 526 208V199Q526 112 465 53Q428 17 388 3T285 -11Q236 -11 195 7T135 43T104 80Q48 165 48 318ZM375 231V244V268Q375 295 373 310T364 342T341 366T299 374H297Q231 374 208 287Q200 257 200 196Q201 120 209 100Q231 47 288 47Q351 47 368 90Q375 112 375 231Z"></path></g><g data-mml-node="mn" transform="translate(575, 0)"><path data-c="35" d="M100 565V605Q100 637 102 646T113 655Q116 655 139 647T202 631T286 623Q332 623 372 631T434 647T459 655Q466 655 469 651T472 643T472 629Q472 613 463 601Q370 487 219 487Q195 487 183 488T169 490T168 433V376Q169 376 174 379T188 387T211 397T244 405T288 409Q390 409 453 352T517 201Q517 106 445 48T253 -11Q169 -11 113 37T57 154Q57 187 79 208T131 229T183 209T206 154Q206 99 155 83Q152 82 157 78Q196 47 253 47Q347 47 358 135Q358 137 358 138Q360 158 360 209Q360 277 355 301T337 338Q315 358 282 358Q202 358 160 303Q153 294 149 292T130 290Q107 290 102 301Q100 304 100 474V565Z"></path></g><g data-mml-node="mo" transform="translate(1150, 0)"><path data-c="2E" d="M74 85Q74 121 99 146T156 171Q200 171 222 143T245 85Q245 56 224 29T160 1Q118 1 96 27T74 85Z"></path></g><g data-mml-node="mn" transform="translate(1635.7, 0)"><path data-c="32" d="M175 580Q175 578 185 572T205 551T215 510Q215 467 191 449T137 430Q107 430 83 448T58 511Q58 558 91 592T168 640T259 654Q328 654 383 637Q451 610 484 563T517 459Q517 401 482 360T368 262Q340 243 265 184L210 140H274Q416 140 429 145Q439 148 447 186T455 237H517V233Q516 230 501 119Q489 9 486 4V0H57V25Q57 51 58 54Q60 57 109 106T215 214T288 291Q364 377 364 458Q364 515 328 553T231 592Q214 592 201 589T181 584T175 580Z"></path></g><g data-mml-node="mn" transform="translate(2210.7, 0)"><path data-c="37" d="M256 -11Q231 -11 208 5T185 65Q185 105 193 146T212 220T241 289T275 349T312 402T346 445T377 479T397 502L400 504H301Q156 503 150 497Q142 491 134 456T126 407H64V411Q65 414 82 544T99 675T130 676H161V673Q161 669 162 666T167 661T173 657T181 654T190 652T200 651T210 650T220 649T229 648Q237 648 254 647T276 646Q277 646 426 644H558V620V607Q558 596 551 586T509 537Q489 515 476 500Q390 401 384 393Q349 339 337 259T324 113T322 38Q307 -11 256 -11Z"></path></g></g></g></g></svg></mjx-container></span></td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; "><span class="math-inline ">
<mjx-container class="MathJax" jax="SVG"><svg style="vertical-align: -0.025ex" xmlns="http://www.w3.org/2000/svg" width="6.302ex" height="1.509ex" role="img" focusable="false" viewBox="0 -656 2785.7 667"><g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)"><g data-mml-node="math"><g data-mml-node="TeXAtom" data-mjx-texclass="ORD"><g data-mml-node="mn"><path data-c="36" d="M48 318Q48 395 68 456T120 553T193 613T273 646T350 655Q425 655 461 616T497 524Q497 485 475 468T428 451Q399 451 378 470T357 521Q357 565 403 588Q375 601 351 601Q313 601 282 584Q242 565 222 526Q199 473 199 367Q201 369 210 380T227 396T246 410T275 422T312 426Q438 426 494 332Q526 285 526 208V199Q526 112 465 53Q428 17 388 3T285 -11Q236 -11 195 7T135 43T104 80Q48 165 48 318ZM375 231V244V268Q375 295 373 310T364 342T341 366T299 374H297Q231 374 208 287Q200 257 200 196Q201 120 209 100Q231 47 288 47Q351 47 368 90Q375 112 375 231Z"></path></g><g data-mml-node="mn" transform="translate(575, 0)"><path data-c="34" d="M531 0Q510 3 381 3Q238 3 214 0H201V62H313V155H32V217L205 434Q342 606 362 630T387 655L391 656Q395 656 401 656T414 656H427Q447 656 451 645Q453 641 453 429V217H542V155H453V62H542V0H531ZM324 217V494L103 218L213 217H324Z"></path></g><g data-mml-node="mo" transform="translate(1150, 0)"><path data-c="2E" d="M74 85Q74 121 99 146T156 171Q200 171 222 143T245 85Q245 56 224 29T160 1Q118 1 96 27T74 85Z"></path></g><g data-mml-node="mn" transform="translate(1635.7, 0)"><path data-c="33" d="M80 503Q80 565 133 610T274 655Q366 655 421 623T491 538Q493 528 493 510Q493 446 453 407T361 348L376 344Q452 324 489 281T526 184Q526 152 514 121T474 58T392 8T265 -11Q175 -11 111 34T48 152Q50 187 72 209T132 232Q171 232 193 208T216 147Q216 136 214 126T207 108T197 94T187 84T178 77T170 72L168 71Q168 70 179 65T215 54T266 48H270Q331 48 350 105Q358 128 358 185Q358 239 348 268T309 313Q292 321 242 322Q205 322 198 324T191 341V348Q191 366 196 369T232 375Q239 375 247 376T260 377T268 378Q284 383 297 393T326 436T341 517Q341 536 339 547T331 573T308 593T266 600Q248 600 241 599Q214 593 183 576Q234 556 234 503Q234 462 210 444T157 426Q126 426 103 446T80 503Z"></path></g><g data-mml-node="mn" transform="translate(2210.7, 0)"><path data-c="33" d="M80 503Q80 565 133 610T274 655Q366 655 421 623T491 538Q493 528 493 510Q493 446 453 407T361 348L376 344Q452 324 489 281T526 184Q526 152 514 121T474 58T392 8T265 -11Q175 -11 111 34T48 152Q50 187 72 209T132 232Q171 232 193 208T216 147Q216 136 214 126T207 108T197 94T187 84T178 77T170 72L168 71Q168 70 179 65T215 54T266 48H270Q331 48 350 105Q358 128 358 185Q358 239 348 268T309 313Q292 321 242 322Q205 322 198 324T191 341V348Q191 366 196 369T232 375Q239 375 247 376T260 377T268 378Q284 383 297 393T326 436T341 517Q341 536 339 547T331 573T308 593T266 600Q248 600 241 599Q214 593 183 576Q234 556 234 503Q234 462 210 444T157 426Q126 426 103 446T80 503Z"></path></g></g></g></g></svg></mjx-container></span></td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; "><span class="math-inline ">
<mjx-container class="MathJax" jax="SVG"><svg style="vertical-align: -0.025ex" xmlns="http://www.w3.org/2000/svg" width="6.302ex" height="1.554ex" role="img" focusable="false" viewBox="0 -676 2785.7 687"><g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)"><g data-mml-node="math"><g data-mml-node="TeXAtom" data-mjx-texclass="ORD"><g data-mml-node="mn"><path data-c="36" d="M48 318Q48 395 68 456T120 553T193 613T273 646T350 655Q425 655 461 616T497 524Q497 485 475 468T428 451Q399 451 378 470T357 521Q357 565 403 588Q375 601 351 601Q313 601 282 584Q242 565 222 526Q199 473 199 367Q201 369 210 380T227 396T246 410T275 422T312 426Q438 426 494 332Q526 285 526 208V199Q526 112 465 53Q428 17 388 3T285 -11Q236 -11 195 7T135 43T104 80Q48 165 48 318ZM375 231V244V268Q375 295 373 310T364 342T341 366T299 374H297Q231 374 208 287Q200 257 200 196Q201 120 209 100Q231 47 288 47Q351 47 368 90Q375 112 375 231Z"></path></g><g data-mml-node="mn" transform="translate(575, 0)"><path data-c="37" d="M256 -11Q231 -11 208 5T185 65Q185 105 193 146T212 220T241 289T275 349T312 402T346 445T377 479T397 502L400 504H301Q156 503 150 497Q142 491 134 456T126 407H64V411Q65 414 82 544T99 675T130 676H161V673Q161 669 162 666T167 661T173 657T181 654T190 652T200 651T210 650T220 649T229 648Q237 648 254 647T276 646Q277 646 426 644H558V620V607Q558 596 551 586T509 537Q489 515 476 500Q390 401 384 393Q349 339 337 259T324 113T322 38Q307 -11 256 -11Z"></path></g><g data-mml-node="mo" transform="translate(1150, 0)"><path data-c="2E" d="M74 85Q74 121 99 146T156 171Q200 171 222 143T245 85Q245 56 224 29T160 1Q118 1 96 27T74 85Z"></path></g><g data-mml-node="mn" transform="translate(1635.7, 0)"><path data-c="30" d="M266 654H280H282Q500 654 524 418Q529 370 529 320Q529 125 456 52Q397 -10 287 -10Q110 -10 63 154Q45 212 45 316Q45 504 113 585Q140 618 185 636T266 654ZM374 548Q347 604 286 604Q247 604 218 575Q197 552 193 511T188 311Q188 159 196 116Q202 87 225 64T287 41Q339 41 367 87Q379 107 382 152T386 329Q386 518 374 548Z"></path></g><g data-mml-node="mn" transform="translate(2210.7, 0)"><path data-c="31" d="M481 0L294 3Q136 3 109 0H96V62H227V304Q227 546 225 546Q169 529 97 529H80V591H97Q231 591 308 647L319 655H333Q355 655 359 644Q361 640 361 351V62H494V0H481Z"></path></g></g></g></g></svg></mjx-container></span></td>
<td style="text-align: center; border-right-style: solid !important; border-right-width: 1px !important; border-bottom-style: solid !important; border-bottom-width: 1px !important; border-top: none !important; width: auto; vertical-align: middle; "><span class="math-inline ">
<mjx-container class="MathJax" jax="SVG"><svg style="vertical-align: -0.025ex" xmlns="http://www.w3.org/2000/svg" width="6.302ex" height="1.507ex" role="img" focusable="false" viewBox="0 -655 2785.7 666"><g stroke="currentColor" fill="currentColor" stroke-width="0" transform="matrix(1 0 0 -1 0 0)"><g data-mml-node="math"><g data-mml-node="TeXAtom" data-mjx-texclass="ORD"><g data-mml-node="mn"><path data-c="36" d="M48 318Q48 395 68 456T120 553T193 613T273 646T350 655Q425 655 461 616T497 524Q497 485 475 468T428 451Q399 451 378 470T357 521Q357 565 403 588Q375 601 351 601Q313 601 282 584Q242 565 222 526Q199 473 199 367Q201 369 210 380T227 396T246 410T275 422T312 426Q438 426 494 332Q526 285 526 208V199Q526 112 465 53Q428 17 388 3T285 -11Q236 -11 195 7T135 43T104 80Q48 165 48 318ZM375 231V244V268Q375 295 373 310T364 342T341 366T299 374H297Q231 374 208 287Q200 257 200 196Q201 120 209 100Q231 47 288 47Q351 47 368 90Q375 112 375 231Z"></path></g><g data-mml-node="mn" transform="translate(575, 0)"><path data-c="35" d="M100 565V605Q100 637 102 646T113 655Q116 655 139 647T202 631T286 623Q332 623 372 631T434 647T459 655Q466 655 469 651T472 643T472 629Q472 613 463 601Q370 487 219 487Q195 487 183 488T169 490T168 433V376Q169 376 174 379T188 387T211 397T244 405T288 409Q390 409 453 352T517 201Q517 106 445 48T253 -11Q169 -11 113 37T57 154Q57 187 79 208T131 229T183 209T206 154Q206 99 155 83Q152 82 157 78Q196 47 253 47Q347 47 358 135Q358 137 358 138Q360 158 360 209Q360 277 355 301T337 338Q315 358 282 358Q202 358 160 303Q153 294 149 292T130 290Q107 290 102 301Q100 304 100 474V565Z"></path></g><g data-mml-node="mo" transform="translate(1150, 0)"><path data-c="2E" d="M74 85Q74 121 99 146T156 171Q200 171 222 143T245 85Q245 56 224 29T160 1Q118 1 96 27T74 85Z"></path></g><g data-mml-node="mn" transform="translate(1635.7, 0)"><path data-c="36" d="M48 318Q48 395 68 456T120 553T193 613T273 646T350 655Q425 655 461 616T497 524Q497 485 475 468T428 451Q399 451 378 470T357 521Q357 565 403 588Q375 601 351 601Q313 601 282 584Q242 565 222 526Q199 473 199 367Q201 369 210 380T227 396T246 410T275 422T312 426Q438 426 494 332Q526 285 526 208V199Q526 112 465 53Q428 17 388 3T285 -11Q236 -11 195 7T135 43T104 80Q48 165 48 318ZM375 231V244V268Q375 295 373 310T364 342T341 366T299 374H297Q231 374 208 287Q200 257 200 196Q201 120 209 100Q231 47 288 47Q351 47 368 90Q375 112 375 231Z"></path></g><g data-mml-node="mn" transform="translate(2210.7, 0)"><path data-c="33" d="M80 503Q80 565 133 610T274 655Q366 655 421 623T491 538Q493 528 493 510Q493 446 453 407T361 348L376 344Q452 324 489 281T526 184Q526 152 514 121T474 58T392 8T265 -11Q175 -11 111 34T48 152Q50 187 72 209T132 232Q171 232 193 208T216 147Q216 136 214 126T207 108T197 94T187 84T178 77T170 72L168 71Q168 70 179 65T215 54T266 48H270Q331 48 350 105Q358 128 358 185Q358 239 348 268T309 313Q292 321 242 322Q205 322 198 324T191 341V348Q191 366 196 369T232 375Q239 375 247 376T260 377T268 378Q284 383 297 393T326 436T341 517Q341 536 339 547T331 573T308 593T266 600Q248 600 241 599Q214 593 183 576Q234 556 234 503Q234 462 210 444T157 426Q126 426 103 446T80 503Z"></path></g></g></g></g></svg></mjx-container></span></td>
</tr>
</tbody>
</table>
