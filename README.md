# Dictionary-API
Scraped Unofficial Dictionary API

### Request Headers
```python
headers = {
    "authority": "content-dictionaryextension-pa.googleapis.com",
    "accept": "*/*",
    "accept-language": "en-US,en;q=0.9",
    "referer": "https://content-dictionaryextension-pa.googleapis.com/static/proxy.html?usegapi=1&jsh=m^%^3B^%^2F_^%^2Fscs^%^2Fabc-static^%^2F_^%^2Fjs^%^2Fk^%^3Dgapi.lb.en.AOzoyjtjrhQ.O^%^2Fd^%^3D1^%^2Frs^%^3DAHpOoo9-fA1P7IZFa1fdRj158NoDqrnbYA^%^2Fm^%^3D__features__",
    "sec-ch-ua-mobile": "?0",
    "sec-fetch-dest": "empty",
    "sec-fetch-mode": "cors",
    "sec-fetch-site": "same-origin",
    "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/119.0.0.0 Safari/537.36",
    "x-client-data": "CI-2yQEIo7bJAQipncoBCI6CywEIlaHLAQia/swBCIWgzQEYj87NARin6s0B",
    "x-clientdetails": "appVersion=5.0^%^20(Windows^%^20NT^%^2010.0^%^3B^%^20Win64^%^3B^%^20x64)^%^20AppleWebKit^%^2F537.36^%^20(KHTML^%^2C^%^20like^%^20Gecko)^%^20Chrome^%^2F119.0.0.0^%^20Safari^%^2F537.36&platform=Win32&userAgent=Mozilla^%^2F5.0^%^20(Windows^%^20NT^%^2010.0^%^3B^%^20Win64^%^3B^%^20x64)^%^20AppleWebKit^%^2F537.36^%^20(KHTML^%^2C^%^20like^%^20Gecko)^%^20Chrome^%^2F119.0.0.0^%^20Safari^%^2F537.36",
    "x-goog-encode-response-if-executable": "base64",
    "x-javascript-user-agent": "google-api-javascript-client/1.1.0",
    "x-origin": "chrome-extension://mgijmajocgfcbeboacabfgobmjgjcoja",
    "x-referer": "chrome-extension://mgijmajocgfcbeboacabfgobmjgjcoja",
    "x-requested-with": "XMLHttpRequest"
}
```

### Url Construct
```python
word = "hello"
url = f"https://content-dictionaryextension-pa.googleapis.com/v1/dictionaryExtensionData?term={word}&language=en&corpus=en-US&country=US&key=AIzaSyA6EEtrDCfBkHV8uU2lgGY-N383ZgAOo7Y"
```
### Fetch Response
```python
import requests
r = requests.get(url=url, headers=headers)
print(r.json())
```
### output
```json
{
  "dictionaryData": [
    {
      "entries": [
        {
          "headword": "hello",
          "etymology": {
            "images": {
              "desktop": {
                "width": 198,
                "height": 96,
                "url": "etymology/en/desktop/c55b20fdbb55636fcc505c5fee313148b9e4a4d9e92592997680616ceb55679b.png"
              },
              "mobile": {
                "width": 291,
                "height": 209,
                "url": "etymology/en/mobile/c55b20fdbb55636fcc505c5fee313148b9e4a4d9e92592997680616ceb55679b.png"
              },
              "tablet": {
                "width": 495,
                "height": 204,
                "url": "etymology/en/tablet/c55b20fdbb55636fcc505c5fee313148b9e4a4d9e92592997680616ceb55679b.png"
              }
            },
            "etymology": {
              "fragments": [
                {
                  "text": "early 19th century: variant of earlier <i>hollo</i> ; related to "
                },
                {
                  "text": "holla",
                  "isEntryLink": true
                },
                {
                  "text": "."
                }
              ],
              "text": "early 19th century: variant of earlier <i>hollo</i> ; related to holla."
            }
          },
          "phonetics": [
            {
              "text": "həˈlō",
              "type": "respell",
              "oxfordAudio": "//ssl.gstatic.com/dictionary/static/sounds/20220808/hello--_us_1_rr.mp3"
            },
            {
              "text": "heˈlō",
              "type": "respell"
            }
          ],
          "senseFamilies": [
            {
              "morphUnits": [
                {
                  "formType": {
                    "posTag": "UH",
                    "description": "exclamation"
                  },
                  "wordForm": "hello"
                },
                {
                  "formType": {
                    "posTag": "UH",
                    "description": "exclamation"
                  },
                  "wordForm": "hallo"
                },
                {
                  "formType": {
                    "posTag": "UH",
                    "description": "exclamation"
                  },
                  "wordForm": "hullo"
                }
              ],
              "senses": [
                {
                  "conciseDefinition": "used as greeting",
                  "exampleGroups": [
                    {
                      "examples": [
                        "hello there, Katie!"
                      ],
                      "scores": [
                        {
                          "fleschReadabilityScore": 62.79,
                          "fleschGradeLevel": 5.2466664
                        }
                      ],
                      "source": "DICTIONARY"
                    }
                  ],
                  "subsenses": [
                    {
                      "conciseDefinition": "used to express surprise",
                      "labelSet": {
                        "geographic": [
                          "British"
                        ]
                      },
                      "exampleGroups": [
                        {
                          "examples": [
                            "hello, what's all this then?"
                          ],
                          "scores": [
                            {
                              "fleschReadabilityScore": 102.045,
                              "fleschGradeLevel": 0.51666665
                            }
                          ],
                          "source": "DICTIONARY"
                        }
                      ],
                      "definition": {
                        "fragments": [
                          {
                            "text": "used to express surprise."
                          }
                        ],
                        "text": "used to express surprise."
                      },
                      "sourceId": "m_en_gbus0460730.017",
                      "wsdSenseIds": [
                        "m_en_us1254307.003"
                      ],
                      "definitionWithComplexWords": {
                        "fragments": [
                          {
                            "text": "used to express surprise."
                          }
                        ],
                        "text": "used to express surprise."
                      }
                    },
                    {
                      "conciseDefinition": "used attract attention",
                      "exampleGroups": [
                        {
                          "examples": [
                            "“Hello below!” he cried"
                          ],
                          "scores": [
                            {
                              "fleschReadabilityScore": 75.875,
                              "fleschGradeLevel": 3.67
                            }
                          ],
                          "source": "DICTIONARY"
                        }
                      ],
                      "definition": {
                        "fragments": [
                          {
                            "text": "used as a cry to attract someone's attention."
                          }
                        ],
                        "text": "used as a cry to attract someone's attention."
                      },
                      "sourceId": "m_en_gbus0460730.018",
                      "wsdSenseIds": [
                        "m_en_us1254307.004"
                      ],
                      "additionalExamples": [
                        "I yelled hello upstairs as I began to head up to see if I could help Mrs. Bishop out."
                      ],
                      "definitionWithComplexWords": {
                        "fragments": [
                          {
                            "text": "used as a cry to attract someone's attention."
                          }
                        ],
                        "text": "used as a cry to attract someone's attention."
                      }
                    },
                    {
                      "conciseDefinition": "used informally to express sarcasm or anger",
                      "exampleGroups": [
                        {
                          "examples": [
                            "Hello! Did you even get what the play was about?"
                          ],
                          "scores": [
                            {
                              "fleschReadabilityScore": 91.78,
                              "fleschGradeLevel": 1.7
                            }
                          ],
                          "source": "DICTIONARY"
                        }
                      ],
                      "definition": {
                        "fragments": [
                          {
                            "text": "expressing sarcasm or anger."
                          }
                        ],
                        "text": "expressing sarcasm or anger."
                      },
                      "sourceId": "m_en_gbus0460730.019",
                      "wsdSenseIds": [
                        "m_en_us1254307.005"
                      ],
                      "additionalExamples": [
                        "Every gathering she beds another partner who isn't her husband, hello!",
                        "Excuse him for picking that awful blue hue - I had always told him to let me pick the color to match with his chestnut-blondish hair, but hello!",
                        "I mean, not that we have that all the time, coz hello!",
                        "My parents are chuckling - I guess more of my reaction than their news, but I mean, hello!",
                        "Over the last two days I have been flooded with porn site IMs… hello!",
                        "She must have been really stupid to have mimicked me… I mean, hello!",
                        "The girl is finding love on the telephone, hello!",
                        "Yeah, that might sound totally rude of me to say, but hello!",
                        "You are supposed to be able to keep up with my voice, hello!"
                      ],
                      "definitionWithComplexWords": {
                        "fragments": [
                          {
                            "text": "expressing "
                          },
                          {
                            "text": "sarcasm",
                            "idfValue": 6.677
                          },
                          {
                            "text": " or anger."
                          }
                        ],
                        "text": "expressing sarcasm or anger."
                      }
                    }
                  ],
                  "definition": {
                    "fragments": [
                      {
                        "text": "used as a greeting or to begin a phone conversation."
                      }
                    ],
                    "text": "used as a greeting or to begin a phone conversation."
                  },
                  "sourceId": "m_en_gbus0460730.012",
                  "wsdSenseIds": [
                    "m_en_us1254307.001"
                  ],
                  "additionalExamples": [
                    "But instead of a normal greeting like saying hello or something, they hugged.",
                    "I was stunned and I said I'm surprised anyone says hello to me ever in the mall or in the store after reading that.",
                    "Logan didn't say hello, but I hadn't expected a greeting.",
                    "Quentin is surprised to see Maggie, and says hello.",
                    "She whispered hello, then began to make her way to her room, where she hoped to take a nap.",
                    "The next day when Daniel came in, she started the normal conversation of ‘Hello, how are you?’ ‘Fine, and you?’",
                    "Tlingit people do not use such greetings as hello, good-bye, good afternoon, or good evening.",
                    "‘Hullo, hullo!’ the first one exclaimed brightly.",
                    "‘Oh, hello,’ she said acting surprised to see the four boys staring at her."
                  ],
                  "definitionWithComplexWords": {
                    "fragments": [
                      {
                        "text": "used as a greeting or to begin a phone conversation."
                      }
                    ],
                    "text": "used as a greeting or to begin a phone conversation."
                  }
                }
              ],
              "partsOfSpeech": [
                {
                  "value": "exclamation"
                }
              ]
            },
            {
              "morphUnits": [
                {
                  "formType": {
                    "posTag": "NN",
                    "description": "noun"
                  },
                  "wordForm": "hello"
                },
                {
                  "formType": {
                    "posTag": "NNS",
                    "description": "plural noun"
                  },
                  "wordForm": "hellos"
                },
                {
                  "formType": {
                    "posTag": "NN",
                    "description": "noun"
                  },
                  "wordForm": "hallo"
                },
                {
                  "formType": {
                    "posTag": "NNS",
                    "description": "plural noun"
                  },
                  "wordForm": "hallos"
                },
                {
                  "formType": {
                    "posTag": "NN",
                    "description": "noun"
                  },
                  "wordForm": "hullo"
                },
                {
                  "formType": {
                    "posTag": "NNS",
                    "description": "plural noun"
                  },
                  "wordForm": "hullos"
                }
              ],
              "senses": [
                {
                  "conciseDefinition": "utterance of ‘hello’",
                  "semanticClasses": [
                    "greeting"
                  ],
                  "exampleGroups": [
                    {
                      "examples": [
                        "she was getting polite nods and hellos from people"
                      ],
                      "scores": [
                        {
                          "fleschReadabilityScore": 75.5,
                          "fleschGradeLevel": 4.9644446
                        }
                      ],
                      "source": "DICTIONARY"
                    }
                  ],
                  "definition": {
                    "fragments": [
                      {
                        "text": "an utterance of “hello”; a greeting."
                      }
                    ],
                    "text": "an utterance of “hello”; a greeting."
                  },
                  "sourceId": "m_en_gbus0460730.025",
                  "kgMapping": {
                    "relatedEntities": [
                      {
                        "targetMid": "/m/0gjq09",
                        "relationType": "EQUIVALENT"
                      }
                    ]
                  },
                  "wsdSenseIds": [
                    "m_en_us1254307.006"
                  ],
                  "additionalExamples": [
                    "He led her to the elevators, nodding hellos to various service people in the lobby.",
                    "I received a few sympathetic smiles and polite hellos.",
                    "Instead, she found herself surrounded by well-dressed, accomplished individuals offering English hellos, hot coffee and fresh pastries.",
                    "It wasn't unusual for her to get happy hellos and welcoming grins, but today was different.",
                    "Riley slowly made her way to the bar greeting various friends and classmates with smiles and brief hellos.",
                    "The band members chuckled at me, nodded their hellos, and went back to warming up.",
                    "They nodded their hellos, Lisa heading straight for business.",
                    "Waving polite hellos, I pretended to listen into what was turning out to be a very boring conversation about stocks and bonds.",
                    "We didn't get the chance to get together this visit, but we had nice phone conversation and a waved hello.",
                    "When our paths just crossed, we gave polite hellos and tight-lipped smiles and then continued on our ways.",
                    "When their eyes met, she grinned wickedly in an informal hello.",
                    "With little more than a hello, I began to reread the letter that was in my hand."
                  ],
                  "definitionWithComplexWords": {
                    "fragments": [
                      {
                        "text": "an "
                      },
                      {
                        "text": "utterance",
                        "idfValue": 8.163
                      },
                      {
                        "text": " of “hello”; a greeting."
                      }
                    ],
                    "text": "an utterance of “hello”; a greeting."
                  }
                }
              ],
              "partsOfSpeech": [
                {
                  "value": "noun"
                }
              ]
            },
            {
              "morphUnits": [
                {
                  "formType": {
                    "posTag": "VB",
                    "description": "verb"
                  },
                  "wordForm": "hello"
                },
                {
                  "formType": {
                    "posTag": "VBZ",
                    "description": "3rd person present"
                  },
                  "wordForm": "helloes"
                },
                {
                  "formType": {
                    "posTag": "VBD",
                    "description": "past tense"
                  },
                  "wordForm": "helloed"
                },
                {
                  "formType": {
                    "posTag": "VBN",
                    "description": "past participle"
                  },
                  "wordForm": "helloed"
                },
                {
                  "formType": {
                    "posTag": "VBG",
                    "description": "gerund or present participle"
                  },
                  "wordForm": "helloing"
                },
                {
                  "formType": {
                    "posTag": "VB",
                    "description": "verb"
                  },
                  "wordForm": "hallo"
                },
                {
                  "formType": {
                    "posTag": "VBZ",
                    "description": "3rd person present"
                  },
                  "wordForm": "halloes"
                },
                {
                  "formType": {
                    "posTag": "VBD",
                    "description": "past tense"
                  },
                  "wordForm": "halloed"
                },
                {
                  "formType": {
                    "posTag": "VBN",
                    "description": "past participle"
                  },
                  "wordForm": "halloed"
                },
                {
                  "formType": {
                    "posTag": "VBG",
                    "description": "gerund or present participle"
                  },
                  "wordForm": "halloing"
                },
                {
                  "formType": {
                    "posTag": "VB",
                    "description": "verb"
                  },
                  "wordForm": "hullo"
                },
                {
                  "formType": {
                    "posTag": "VBZ",
                    "description": "3rd person present"
                  },
                  "wordForm": "hulloes"
                },
                {
                  "formType": {
                    "posTag": "VBD",
                    "description": "past tense"
                  },
                  "wordForm": "hulloed"
                },
                {
                  "formType": {
                    "posTag": "VBN",
                    "description": "past participle"
                  },
                  "wordForm": "hulloed"
                },
                {
                  "formType": {
                    "posTag": "VBG",
                    "description": "gerund or present participle"
                  },
                  "wordForm": "hulloing"
                }
              ],
              "senses": [
                {
                  "conciseDefinition": "say or shout ‘hello’",
                  "exampleGroups": [
                    {
                      "examples": [
                        "I pressed the phone button and helloed"
                      ],
                      "scores": [
                        {
                          "fleschReadabilityScore": 90.95857,
                          "fleschGradeLevel": 2.3114285
                        }
                      ],
                      "source": "DICTIONARY"
                    }
                  ],
                  "definition": {
                    "fragments": [
                      {
                        "text": "say or shout “hello”; greet someone."
                      }
                    ],
                    "text": "say or shout “hello”; greet someone."
                  },
                  "sourceId": "m_en_gbus0460730.034",
                  "wsdSenseIds": [
                    "m_en_us1254307.007"
                  ],
                  "additionalExamples": [
                    "He halloed me back and set about making some more porridge.",
                    "‘Hi Kirsten,’ he helloed, obviously calling me Kirsten on purpose."
                  ],
                  "definitionWithComplexWords": {
                    "fragments": [
                      {
                        "text": "say or "
                      },
                      {
                        "text": "shout",
                        "idfValue": 5.559
                      },
                      {
                        "text": " “hello”; "
                      },
                      {
                        "text": "greet",
                        "idfValue": 5.843
                      },
                      {
                        "text": " someone."
                      }
                    ],
                    "text": "say or shout “hello”; greet someone."
                  }
                }
              ],
              "partsOfSpeech": [
                {
                  "value": "verb"
                }
              ]
            }
          ],
          "syllabifiedHeadword": "hel·lo",
          "locale": "en-US",
          "headwordMatchesUserQuery": true,
          "entrySeqNo": 3625100,
          "sourceId": "m_en_gbus0460730",
          "corpus": {
            "name": "en-US",
            "language": "en"
          },
          "idfValue": 2.918
        }
      ],
      "queryTerm": "hello",
      "usageOverTimeImage": {
        "desktop": {
          "width": 512,
          "height": 120,
          "url": "ngram/en/desktop/9e46e72cd810846765ce5f662d6ea334eec921c7.png"
        },
        "mobile": {
          "width": 544,
          "height": 120,
          "url": "ngram/en/mobile/9e46e72cd810846765ce5f662d6ea334eec921c7.png"
        },
        "tablet": {
          "width": 1040,
          "height": 240,
          "url": "ngram/en/tablet/9e46e72cd810846765ce5f662d6ea334eec921c7.png"
        }
      }
    }
  ],
  "status": 200
}
```
