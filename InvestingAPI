{
  "_": {
    "postman_id": "8d1185ea-d3ac-490b-b848-37972e5be0d6"
  },
  "item": [
    {
      "id": "f34cb42a-ebec-44a6-b52c-c489b518cddd",
      "name": "Authentication APIs",
      "item": [
        {
          "id": "90ccd3bd-4274-4ce4-b7af-695ba6446bf6",
          "name": "Auth",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "71fea241-7981-49be-a5ae-a2815720df69",
              "name": "Create Session Token",
              "request": {
                "name": "Create Session Token",
                "description": {
                  "content": "Creates a session token for an implementer to utilize for subsequent API requests.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "auth",
                    "tokens"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "POST",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"clientID\": \"{{dwClientID}}\",\n  \"clientSecret\": \"{{dwClientSecret}}\"\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "f67c27c7-d094-474d-9c2d-6566d09dcf26",
                  "name": "Creating Session Token was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "auth",
                        "tokens"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"clientID\": \"0oafccTendies67BTx113\",\n  \"clientSecret\": \"8WfNzC4oTendiesTradingCompanyPuQNwg7BPByWqQOj\"\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"token_type\": \"Bearer\",\n  \"expires_in\": \"3600\",\n  \"access_token\": \"eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c\",\n  \"scope\": \"all_trading\"\n}",
                  "cookie": []
                }
              ],
              "event": [
                {
                  "listen": "test",
                  "script": {
                    "id": "b6bdbbee-8d87-47e0-b0c7-e42b0de86262",
                    "type": "text/javascript",
                    "exec": [
                      "var response = pm.response.json();\npm.environment.set('dwToken', response.access_token);\npm.environment.set(\"dwTokenExpiry\", Date.now() + response.expires_in * 1000)\n\t\t\t\t\t\t\t"
                    ]
                  }
                }
              ],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        }
      ],
      "event": [],
      "auth": {
        "type": "noauth",
        "noauth": []
      }
    },
    {
      "id": "3b2388e1-8d06-40d0-a7dc-fc59f59eac5c",
      "name": "Core APIs",
      "item": [
        {
          "id": "8bee619c-8b92-4657-a4c4-e0409c07ce63",
          "name": "Users",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "af7c0fc3-ce51-4c8c-ac9a-7e030b87839a",
              "name": "Create User",
              "request": {
                "name": "Create User",
                "description": {
                  "content": "Creates a User.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "users"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "POST",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"userType\": \"<string>\",\n  \"documents\": [\n    {\n      \"type\": \"<string>\",\n      \"data\": {\n        \"firstName\": \"<string>\",\n        \"lastName\": \"<string>\",\n        \"country\": \"<string>\",\n        \"phone\": \"<string>\",\n        \"emailAddress\": \"<string>\",\n        \"language\": \"<string>\"\n      }\n    },\n    {\n      \"type\": \"<string>\",\n      \"data\": {\n        \"firstName\": \"<string>\",\n        \"lastName\": \"<string>\",\n        \"country\": \"<string>\",\n        \"phone\": \"<string>\",\n        \"emailAddress\": \"<string>\",\n        \"language\": \"<string>\"\n      }\n    }\n  ],\n  \"metadata\": \"<object>\"\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "59eae2e9-fac8-49af-89da-962640806560",
                  "name": "Creating a User was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "users"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"userType\": \"INDIVIDUAL_TRADER\",\n  \"documents\": [\n    {\n      \"type\": \"BASIC_INFO\",\n      \"data\": {\n        \"firstName\": \"Justin\",\n        \"lastName\": \"Smith\",\n        \"country\": \"USA\",\n        \"phone\": \"18004612680\",\n        \"emailAddress\": \"jj@drivewealth.dev\",\n        \"language\": \"en_US\"\n      }\n    },\n    {\n      \"type\": \"BASIC_INFO\",\n      \"data\": {\n        \"firstName\": \"Justin\",\n        \"lastName\": \"Smith\",\n        \"country\": \"USA\",\n        \"phone\": \"18004612680\",\n        \"emailAddress\": \"jj@drivewealth.dev\",\n        \"language\": \"en_US\"\n      }\n    }\n  ],\n  \"metadata\": {\n    \"myCustomKey\": \"myCustomValue\"\n  }\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n  \"userType\": {\n    \"name\": \"INDIVIDUAL_TRADER\",\n    \"description\": \"Individual Trader\"\n  },\n  \"status\": {\n    \"name\": \"PENDING\",\n    \"description\": \"User is pending approval.\"\n  },\n  \"parentIBID\": {\n    \"id\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9\",\n    \"name\": \"Tendies Trading Company\"\n  },\n  \"documents\": [\n    {\n      \"type\": \"BASIC_INFO\",\n      \"data\": {\n        \"firstName\": \"Justin\",\n        \"lastName\": \"Smith\",\n        \"country\": \"USA\",\n        \"phone\": \"18004612680\",\n        \"emailAddress\": \"jj@drivewealth.dev\",\n        \"language\": \"en_US\"\n      }\n    },\n    {\n      \"type\": \"BASIC_INFO\",\n      \"data\": {\n        \"firstName\": \"Justin\",\n        \"lastName\": \"Smith\",\n        \"country\": \"USA\",\n        \"phone\": \"18004612680\",\n        \"emailAddress\": \"jj@drivewealth.dev\",\n        \"language\": \"en_US\"\n      }\n    }\n  ],\n  \"wlpID\": \"TTC\",\n  \"referralCode\": \"71J000\",\n  \"createdWhen\": \"2022-12-11T22:28:21.810Z\",\n  \"updatedWhen\": \"2022-12-11T22:28:21.810Z\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "03398bee-3655-480b-8374-267d341eb995",
              "name": "Retrieve User",
              "request": {
                "name": "Retrieve User",
                "description": {
                  "content": "Retrieves a User details by userID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "users",
                    ":userID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) Unique ID of the User to fetch.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "userID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "420830ee-707b-444a-a7b1-bb600ddbb2f4",
                  "name": "Retrieving a User was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "users",
                        ":userID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) Unique ID of the User to fetch.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "userID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"user\": {\n    \"id\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n    \"ackSignedWhen\": \"2022-12-11T22:28:21.666Z\",\n    \"addressLine1\": \"15 Exchange Place\",\n    \"addressLine2\": \"Suite 1000\",\n    \"city\": \"Jersey City\",\n    \"countryID\": \"USA\",\n    \"displayName\": \"JSmith\",\n    \"dob\": \"2000-12-3\",\n    \"email\": \"jj@drivewealth.dev\",\n    \"firstName\": \"Justin\",\n    \"gender\": {\n      \"name\": \"MALE\"\n    },\n    \"languageID\": \"en_US\",\n    \"lastname\": \"Smith\",\n    \"parentIBID\": {\n      \"id\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9\",\n      \"name\": \"Tendies Trading Company\"\n    },\n    \"phone\": \"18004612680\",\n    \"referralCode\": \"71J000\",\n    \"stateProvince\": \"NJ\",\n    \"wlpID\": \"TTC\",\n    \"zipPostalCode\": \"magna Ut\",\n    \"idNo\": \"****-4444\",\n    \"status\": {\n      \"name\": \"PENDING\",\n      \"description\": \"User is pending approval.\"\n    },\n    \"userType\": {\n      \"name\": \"INDIVIDUAL_TRADER\",\n      \"description\": \"Individual Trader\"\n    },\n    \"usCitizen\": true,\n    \"updatedWhen\": \"2022-12-11T22:28:21.810Z\",\n    \"brandAmbassador\": false,\n    \"employerBusiness\": \"FINANCE\",\n    \"employementStatus\": {\n      \"name\": \"EMPLOYED\",\n      \"description\": \"Employed\"\n    },\n    \"citizenship\": \"USA\",\n    \"createdWhen\": \"2022-12-11T22:28:21.810Z\",\n    \"marginDefault\": 0,\n    \"maritalStatus\": {\n      \"name\": \"SINGLE\",\n      \"description\": \"Single\"\n    },\n    \"ackCustomerAgreement\": true,\n    \"ackFixedIncomeAgreement\": false,\n    \"ackFindersFee\": false,\n    \"ackForeignFindersFee\": false,\n    \"ackJointCustomerAgreement\": true,\n    \"ackJointFindersFee\": false,\n    \"ackJointForeignFindersFee\": false,\n    \"ackJointMarketData\": false,\n    \"ackMarketData\": false,\n    \"ackExtendedHoursAgreement\": false,\n    \"ackOptionsAgreement\": true,\n    \"dependents\": 0,\n    \"termsOfUse\": true,\n    \"badPasswordCount\": false,\n    \"director\": false,\n    \"employerCompany\": \"DriveWealth LLC\",\n    \"employerCompanyID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n    \"employerCompanyStartDate\": \"2014-09-29\",\n    \"employerCompanyEndDate\": \"2022-12-25\",\n    \"employerIsBroker\": true,\n    \"employmentPosition\": \"ENGINEER\",\n    \"employmentYears\": 0,\n    \"jointEmployerIsBroker\": false,\n    \"investmentObjectives\": {\n      \"name\": \"FREQUENT\",\n      \"description\": \"Frequent trader, depending on the market\"\n    },\n    \"investmentExperience\": {\n      \"name\": \"YRS_10_\",\n      \"description\": \"10+ yrs\"\n    },\n    \"politicallyExposed\": false,\n    \"riskTolerance\": \"HIGH\",\n    \"userNoteQty\": 0,\n    \"validTaxForm\": true,\n    \"taxTreatyWithUS\": true,\n    \"avatarURL\": \"https://secure.gravatar.com/avatar/2076105f6efe7c11e285add95f514b9a.jpg\",\n    \"annualIncomeRange\": \"$0 - $24,999\",\n    \"ackDisclosureRule14b\": true,\n    \"ackJointDisclosureRule14b\": false,\n    \"networthLiquidRange\": \"Unknown\",\n    \"networthTotalRange\": \"$200,000 - $499,999\",\n    \"investmentEquitiesExperience\": \"LIMITED\",\n    \"investmentEquitiesYears\": \"YRS_10_PLUS\",\n    \"investmentEquitiesTradesPerYear\": \"YRS_10_14\",\n    \"investmentEquitiesAverageTradeSize\": \"AVG_0_9999\",\n    \"investmentOptionsExperience\": \"LIMITED\",\n    \"investmentOptionsYears\": \"YRS_10_PLUS\",\n    \"investmentOptionsTradesPerYear\": \"YRS_10_14\",\n    \"investmentOptionsAverageTradeSize\": \"AVG_0_9999\"\n  }\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "3740e959-2d46-465d-add4-a6e535443d9b",
              "name": "Update User",
              "request": {
                "name": "Update User",
                "description": {
                  "content": "Updates a User details by userID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "users",
                    ":userID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) Unique ID of the User to update.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "userID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "PATCH",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"documents\": [\n    {\n      \"type\": \"<string>\",\n      \"data\": {\n        \"firstName\": \"<string>\",\n        \"lastName\": \"<string>\",\n        \"country\": \"<string>\",\n        \"phone\": \"<string>\",\n        \"emailAddress\": \"<string>\",\n        \"language\": \"<string>\"\n      }\n    },\n    {\n      \"type\": \"<string>\",\n      \"data\": {\n        \"firstName\": \"<string>\",\n        \"lastName\": \"<string>\",\n        \"country\": \"<string>\",\n        \"phone\": \"<string>\",\n        \"emailAddress\": \"<string>\",\n        \"language\": \"<string>\"\n      }\n    }\n  ]\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "7d745eb8-9931-495a-88c9-1470b2681176",
                  "name": "Fetching a User is Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "users",
                        ":userID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) Unique ID of the User to update.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "userID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "PATCH",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"documents\": [\n    {\n      \"type\": \"BASIC_INFO\",\n      \"data\": {\n        \"firstName\": \"Justin\",\n        \"lastName\": \"Smith\",\n        \"country\": \"USA\",\n        \"phone\": \"18004612680\",\n        \"emailAddress\": \"jj@drivewealth.dev\",\n        \"language\": \"en_US\"\n      }\n    },\n    {\n      \"type\": \"BASIC_INFO\",\n      \"data\": {\n        \"firstName\": \"Justin\",\n        \"lastName\": \"Smith\",\n        \"country\": \"USA\",\n        \"phone\": \"18004612680\",\n        \"emailAddress\": \"jj@drivewealth.dev\",\n        \"language\": \"en_US\"\n      }\n    }\n  ]\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n  \"ackSignedWhen\": \"2022-12-11T22:28:21.666Z\",\n  \"addressLine1\": \"15 Exchange Place\",\n  \"addressLine2\": \"Suite 1000\",\n  \"city\": \"Jersey City\",\n  \"countryID\": \"USA\",\n  \"displayName\": \"JSmith\",\n  \"dob\": \"2000-12-3\",\n  \"email\": \"jj@drivewealth.dev\",\n  \"firstName\": \"Justin\",\n  \"gender\": {\n    \"name\": \"MALE\"\n  },\n  \"languageID\": \"en_US\",\n  \"lastname\": \"Smith\",\n  \"parentIBID\": {\n    \"id\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9\",\n    \"name\": \"Tendies Trading Company\"\n  },\n  \"phone\": \"18004612680\",\n  \"referralCode\": \"71J000\",\n  \"stateProvince\": \"NJ\",\n  \"wlpID\": \"TTC\",\n  \"zipPostalCode\": \"94105\",\n  \"idNo\": \"****-4444\",\n  \"status\": {\n    \"name\": \"PENDING\",\n    \"description\": \"User is pending approval.\"\n  },\n  \"userType\": {\n    \"name\": \"INDIVIDUAL_TRADER\",\n    \"description\": \"Individual Trader\"\n  },\n  \"usCitizen\": true,\n  \"updatedWhen\": \"2022-12-11T22:28:21.810Z\",\n  \"brandAmbassador\": false,\n  \"employerBusiness\": \"FINANCE\",\n  \"employementStatus\": {\n    \"name\": \"EMPLOYED\",\n    \"description\": \"Employed\"\n  },\n  \"citizenship\": \"US\",\n  \"createdWhen\": \"2022-12-11T22:28:21.810Z\",\n  \"marginDefault\": 0,\n  \"maritalStatus\": {\n    \"name\": \"SINGLE\",\n    \"description\": \"Single\"\n  },\n  \"ackCustomerAgreement\": true,\n  \"ackFindersFee\": false,\n  \"ackFixedIncomeAgreement\": true,\n  \"ackForeignFindersFee\": false,\n  \"ackJointCustomerAgreement\": true,\n  \"ackJointFindersFee\": false,\n  \"ackJointForeignFindersFee\": false,\n  \"ackJointMarketData\": false,\n  \"ackMarketData\": false,\n  \"ackExtendedHoursAgreement\": false,\n  \"ackOptionsAgreement\": true,\n  \"dependents\": 0,\n  \"termsOfUse\": true,\n  \"director\": false,\n  \"employerCompany\": \"DriveWealth LLC\",\n  \"employerCompanyID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n  \"employerCompanyStartDate\": \"2014-09-29\",\n  \"employerCompanyEndDate\": \"2022-12-25\",\n  \"employerIsBroker\": true,\n  \"employmentPosition\": \"ENGINEER\",\n  \"employmentYears\": 0,\n  \"jointEmployerIsBroker\": false,\n  \"investmentObjectives\": {\n    \"name\": \"FREQUENT\",\n    \"description\": \"Frequent trader, depending on the market\"\n  },\n  \"investmentExperience\": {\n    \"name\": \"YRS_10_\",\n    \"description\": \"10+ yrs\"\n  },\n  \"politicallyExposed\": false,\n  \"riskTolerance\": \"HIGH\",\n  \"userNoteQty\": 0,\n  \"validTaxForm\": false,\n  \"taxTreatyWithUS\": true,\n  \"avatarURL\": \"https://secure.gravatar.com/avatar/2076105f6efe7c11e285add95f514b9a.jpg\",\n  \"annualIncomeRange\": \"$0 - $24,999\",\n  \"ackDisclosureRule14b\": true,\n  \"ackJointDisclosureRule14b\": false,\n  \"networthLiquidRange\": \"$0 - $24,999\",\n  \"networthTotalRange\": \"$0 - $24,999\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "274699b9-ad4b-4e29-917a-1bf6ae7fe7a9",
              "name": "Retrieve KYC",
              "request": {
                "name": "Retrieve KYC",
                "description": {
                  "content": "Retrives a User KYC by userID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "users",
                    ":userID",
                    "kyc-status"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) Unique ID of the User to fetch their profile & kyc status.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "userID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "9ed74a08-b60f-4a68-9895-408fe286875c",
                  "name": "Fetching User's Profile Details & KYC is Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "users",
                        ":userID",
                        "kyc-status"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) Unique ID of the User to fetch their profile & kyc status.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "userID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n  \"firstName\": \"Justin\",\n  \"lastName\": \"Smith\",\n  \"identity\": {\n    \"number\": \"****-4444\",\n    \"dob\": \"2000-12-03\"\n  },\n  \"accounts\": [\n    {\n      \"id\": \"8b8ba3fd-74dc-45dc-b2dc-7de683bd713c.1556222995391\",\n      \"accountNo\": \"DWBG000052\",\n      \"nickname\": \"Justin's Self Directed Account\",\n      \"accountStatus\": {\n        \"name\": \"PENDING\",\n        \"description\": \"Pending\"\n      },\n      \"accountType\": \"LIVE\",\n      \"accountManagementType\": \"SELF\",\n      \"tradingType\": \"CASH\",\n      \"leverage\": 1\n    },\n    {\n      \"id\": \"8b8ba3fd-74dc-45dc-b2dc-7de683bd713c.1556222995391\",\n      \"accountNo\": \"DWBG000052\",\n      \"nickname\": \"Justin's Self Directed Account\",\n      \"accountStatus\": {\n        \"name\": \"PENDING\",\n        \"description\": \"Pending\"\n      },\n      \"accountType\": \"LIVE\",\n      \"accountManagementType\": \"SELF\",\n      \"tradingType\": \"CASH\",\n      \"leverage\": 1\n    }\n  ],\n  \"kyc\": {\n    \"status\": {\n      \"name\": \"KYC_INFO_REQUIRED\",\n      \"code\": \"K102\",\n      \"description\": \"User's PII not matched. Please revisit user's PII Info.\"\n    },\n    \"approved\": {\n      \"timestamp\": \"2022-12-12T21:13:12.391Z\",\n      \"approvedBy\": \"0ef9ef36-3720-4b76-a938-dac4501a7f95\"\n    },\n    \"accepted\": {\n      \"acceptedBy\": \"SYSTEM PRINCIPAL APPROVER\",\n      \"timeStamp\": \"2022-12-12T21:13:12.391Z\"\n    }\n  },\n  \"status\": {\n    \"name\": \"APPROVED\",\n    \"description\": \"User approved.\"\n  },\n  \"partnerID\": {\n    \"id\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9\",\n    \"name\": \"Tendies Trading Company\"\n  }\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "cfc34e1f-6783-4de7-b762-c62f628373c9",
          "name": "Disclosures",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [],
          "event": []
        },
        {
          "id": "e1b50a5d-a0d7-44c8-b679-4b376362973a",
          "name": "Accounts",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "d9db5496-0340-4bb2-be99-e1afba839ed3",
              "name": "Create Account",
              "request": {
                "name": "Create Account",
                "description": {
                  "content": "Creates a trading Account.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "POST",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"userID\": \"<string>\",\n  \"accountType\": \"<string>\",\n  \"accountManagementType\": \"<string>\",\n  \"tradingType\": \"<string>\",\n  \"accountHolderType\": \"<string>\",\n  \"finra3210ComplianceEntity\": \"<string>\",\n  \"riaUserID\": \"<string>\",\n  \"riaProductID\": \"<string>\",\n  \"riaPortfolioID\": \"<string>\",\n  \"authorizedUsers\": [\n    {\n      \"userID\": \"<string>\",\n      \"permissions\": [\n        \"<string>\",\n        \"<string>\"\n      ]\n    },\n    {\n      \"userID\": \"<string>\",\n      \"permissions\": [\n        \"<string>\",\n        \"<string>\"\n      ]\n    }\n  ],\n  \"ignoreBuyingPower\": \"<boolean>\",\n  \"violationsExempt\": \"<boolean>\",\n  \"ignoreMarketHoursForTest\": \"<boolean>\",\n  \"extendedHoursEnrolled\": \"<boolean>\",\n  \"metadata\": \"<object>\",\n  \"leverage\": \"<number>\",\n  \"accountFeatures\": {\n    \"options\": {\n      \"enrolled\": \"<boolean>\",\n      \"optionsLevel\": \"<string>\"\n    },\n    \"mutualFunds\": {\n      \"dividendReinvestment\": \"<boolean>\",\n      \"capitalGainsReinvestment\": \"<boolean>\"\n    },\n    \"fixedIncome\": {\n      \"enrolled\": false\n    },\n    \"equities\": {\n      \"dividendReinvestment\": \"<boolean>\",\n      \"capitalGainsReinvestment\": \"<boolean>\"\n    }\n  },\n  \"interestedParties\": [\n    {\n      \"type\": \"<string>\",\n      \"data\": [\n        {\n          \"id\": \"<string>\",\n          \"reportingRole\": \"<string>\",\n          \"tradeDiscretion\": \"<boolean>\",\n          \"from\": \"<dateTime>\",\n          \"to\": \"<dateTime>\",\n          \"endReason\": \"<string>\"\n        },\n        {\n          \"id\": \"<string>\",\n          \"reportingRole\": \"<string>\",\n          \"tradeDiscretion\": \"<boolean>\",\n          \"from\": \"<dateTime>\",\n          \"to\": \"<dateTime>\",\n          \"endReason\": \"<string>\"\n        }\n      ]\n    },\n    {\n      \"type\": \"<string>\",\n      \"data\": [\n        {\n          \"id\": \"<string>\",\n          \"reportingRole\": \"<string>\",\n          \"tradeDiscretion\": \"<boolean>\",\n          \"from\": \"<dateTime>\",\n          \"to\": \"<dateTime>\",\n          \"endReason\": \"<string>\"\n        },\n        {\n          \"id\": \"<string>\",\n          \"reportingRole\": \"<string>\",\n          \"tradeDiscretion\": \"<boolean>\",\n          \"from\": \"<dateTime>\",\n          \"to\": \"<dateTime>\",\n          \"endReason\": \"<string>\"\n        }\n      ]\n    }\n  ]\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "b53414a0-bcac-40bd-98c4-6f7180a3972d",
                  "name": "Creating an Account was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n  \"accountType\": \"LIVE\",\n  \"accountManagementType\": \"SELF\",\n  \"tradingType\": \"CASH\"\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n  \"accountNo\": \"DWBG000052\",\n  \"accountType\": {\n    \"name\": \"LIVE\",\n    \"description\": \"Live Account\"\n  },\n  \"accountMgmtType\": {\n    \"name\": \"SELF\",\n    \"description\": \"Self Directed Account\"\n  },\n  \"accountHolderType\": {\n    \"name\": \"I\",\n    \"description\": \"An account that does not meet FINRA Rule 4215(c) or a proprietary trading account\"\n  },\n  \"status\": {\n    \"name\": \"OPEN\",\n    \"description\": \"Open\"\n  },\n  \"tradingType\": {\n    \"name\": \"CASH\",\n    \"description\": \"Cash Account\"\n  },\n  \"leverage\": 1,\n  \"nickname\": \"Steve's Robo Advisor Managed Account\",\n  \"parentIB\": {\n    \"id\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9\",\n    \"name\": \"Tendies Trading Company\"\n  },\n  \"taxProfile\": {\n    \"taxStatusCode\": \"W-9\",\n    \"taxRecipientCode\": \"INDIVIDUAL\"\n  },\n  \"commissionID\": \"b3e985dd-9679-63dc-5dd5-9bd7982efecd\",\n  \"beneficiaries\": false,\n  \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n  \"restricted\": false,\n  \"goodFaithViolations\": 0,\n  \"patternDayTrades\": 0,\n  \"freeTradeBalance\": 0,\n  \"gfvPdtExempt\": false,\n  \"buyingPowerOverride\": false,\n  \"bod\": {\n    \"moneyMarket\": 0,\n    \"equityValue\": 0,\n    \"cashAvailableForWithdrawal\": 0,\n    \"cashAvailableForTrading\": 0,\n    \"cashBalance\": 0\n  },\n  \"ria\": {\n    \"advisorID\": \"66304da9-3h6f-2234-935f-ac6b7933d706\",\n    \"productID\": \"product_b94c0b6a-5ac8-43e4-95d1-777051c0503b\"\n  },\n  \"sweepInd\": true,\n  \"interestFree\": false,\n  \"openedWhen\": \"2022-12-22T06:07:41Z\",\n  \"ignoreMarketHoursForTest\": false,\n  \"flaggedForACATS\": false,\n  \"accountFeatures\": {\n    \"options\": {\n      \"enrolled\": \"<boolean>\",\n      \"optionsLevel\": \"LEVEL_1\"\n    },\n    \"mutualFunds\": {\n      \"dividendReinvestment\": true,\n      \"dividendReinvestmentOptInWhen\": \"2022-12-11T22:28:21.810Z\",\n      \"dividendReinvestmentOptOutWhen\": \"2022-12-11T22:28:21.810Z\",\n      \"capitalGainsReinvestment\": true,\n      \"capitalGainsReinvestmentOptInWhen\": \"2022-12-11T22:28:21.810Z\",\n      \"capitalGainsReinvestmentOptOutWhen\": \"2022-12-11T22:28:21.810Z\"\n    },\n    \"fixedIncome\": {\n      \"enrolled\": true\n    },\n    \"equities\": {\n      \"dividendReinvestment\": true,\n      \"dividendReinvestmentOptInWhen\": \"2022-12-11T22:28:21.810Z\",\n      \"dividendReinvestmentOptOutWhen\": \"2022-12-11T22:28:21.810Z\",\n      \"capitalGainsReinvestment\": true,\n      \"capitalGainsReinvestmentOptInWhen\": \"2022-12-11T22:28:21.810Z\",\n      \"capitalGainsReinvestmentOptOutWhen\": \"2022-12-11T22:28:21.810Z\"\n    }\n  },\n  \"interestedParties\": [\n    {\n      \"type\": \"<string>\",\n      \"data\": [\n        {\n          \"id\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n          \"reportingRole\": \"<string>\",\n          \"tradeDiscretion\": \"<boolean>\",\n          \"from\": \"<dateTime>\",\n          \"to\": \"<dateTime>\",\n          \"endReason\": \"<string>\"\n        },\n        {\n          \"id\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n          \"reportingRole\": \"<string>\",\n          \"tradeDiscretion\": \"<boolean>\",\n          \"from\": \"<dateTime>\",\n          \"to\": \"<dateTime>\",\n          \"endReason\": \"<string>\"\n        }\n      ]\n    },\n    {\n      \"type\": \"<string>\",\n      \"data\": [\n        {\n          \"id\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n          \"reportingRole\": \"<string>\",\n          \"tradeDiscretion\": \"<boolean>\",\n          \"from\": \"<dateTime>\",\n          \"to\": \"<dateTime>\",\n          \"endReason\": \"<string>\"\n        },\n        {\n          \"id\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n          \"reportingRole\": \"<string>\",\n          \"tradeDiscretion\": \"<boolean>\",\n          \"from\": \"<dateTime>\",\n          \"to\": \"<dateTime>\",\n          \"endReason\": \"<string>\"\n        }\n      ]\n    }\n  ]\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "f6fcabf7-43a8-4383-bad4-b68691505e7f",
              "name": "Retrieve Account",
              "request": {
                "name": "Retrieve Account",
                "description": {
                  "content": "Retrieves an Account details by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "633e16ed-7770-4029-8677-8853581f8b81",
                  "name": "Retrieving Account details was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"account\": {\n    \"id\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n    \"accountNo\": \"DWBG000052\",\n    \"accountType\": {\n      \"name\": \"LIVE\",\n      \"description\": \"Live Account\"\n    },\n    \"accountMgmtType\": {\n      \"name\": \"SELF\",\n      \"description\": \"Self Directed Account\"\n    },\n    \"accountHolderType\": {\n      \"name\": \"I\",\n      \"description\": \"An account that does not meet FINRA Rule 4215(c) or a proprietary trading account\"\n    },\n    \"finra3210ComplianceEntity\": \"COMPLYSCI\",\n    \"status\": {\n      \"name\": \"OPEN\",\n      \"description\": \"Open\"\n    },\n    \"tradingType\": {\n      \"name\": \"CASH\",\n      \"description\": \"Cash Account\"\n    },\n    \"leverage\": 1,\n    \"nickname\": \"Steve's Robo Advisor Managed Account\",\n    \"parentIB\": {\n      \"id\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9\",\n      \"name\": \"Tendies Trading Company\"\n    },\n    \"taxProfile\": {\n      \"taxStatusCode\": \"W-9\",\n      \"taxRecipientCode\": \"INDIVIDUAL\"\n    },\n    \"commissionID\": \"b3e985dd-9679-63dc-5dd5-9bd7982efecd\",\n    \"beneficiaries\": false,\n    \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n    \"restricted\": false,\n    \"gfvRestricted\": false,\n    \"goodFaithViolations\": 0,\n    \"pdtRestricted\": false,\n    \"patternDayTrader\": false,\n    \"patternDayTrades\": 0,\n    \"freeTradeBalance\": 0,\n    \"gfvPdtExempt\": false,\n    \"buyingPowerOverride\": false,\n    \"bod\": {\n      \"moneyMarket\": 0,\n      \"equityValue\": 0,\n      \"cashAvailableForWithdrawal\": 0,\n      \"cashAvailableForTrading\": 0,\n      \"cashBalance\": 0\n    },\n    \"ria\": {\n      \"advisorID\": \"66304da9-3h6f-2234-935f-ac6b7933d706\",\n      \"productID\": \"product_b94c0b6a-5ac8-43e4-95d1-777051c0503b\"\n    },\n    \"sweepInd\": true,\n    \"interestFree\": false,\n    \"accountFeatures\": {\n      \"options\": {\n        \"enrolled\": \"<boolean>\",\n        \"optionsLevel\": \"LEVEL_1\"\n      },\n      \"mutualFunds\": {\n        \"dividendReinvestment\": true,\n        \"dividendReinvestmentOptInWhen\": \"2022-12-11T22:28:21.810Z\",\n        \"dividendReinvestmentOptOutWhen\": \"2022-12-11T22:28:21.810Z\",\n        \"capitalGainsReinvestment\": true,\n        \"capitalGainsReinvestmentOptInWhen\": \"2022-12-11T22:28:21.810Z\",\n        \"capitalGainsReinvestmentOptOutWhen\": \"2022-12-11T22:28:21.810Z\"\n      },\n      \"fixedIncome\": {\n        \"enrolled\": true\n      },\n      \"equities\": {\n        \"dividendReinvestment\": true,\n        \"dividendReinvestmentOptInWhen\": \"2022-12-11T22:28:21.810Z\",\n        \"dividendReinvestmentOptOutWhen\": \"2022-12-11T22:28:21.810Z\",\n        \"capitalGainsReinvestment\": true,\n        \"capitalGainsReinvestmentOptInWhen\": \"2022-12-11T22:28:21.810Z\",\n        \"capitalGainsReinvestmentOptOutWhen\": \"2022-12-11T22:28:21.810Z\"\n      }\n    },\n    \"statusChangeReason\": \"LEGAL_AML\",\n    \"statusUpdatedBy\": \"ACAT_SYSTEM\",\n    \"statusChangeHistory\": {\n      \"status\": \"OPEN\",\n      \"statusChangeReason\": \"LEGAL_AML\",\n      \"statusUpdatedBy\": \"ACAT_SYSTEM\"\n    },\n    \"createdWhen\": \"2022-12-22T06:07:41.773Z\",\n    \"openedWhen\": \"2022-12-22T06:07:41Z\",\n    \"updatedWhen\": \"2022-12-22T16:04:47.140Z\",\n    \"ignoreMarketHoursForTest\": false,\n    \"flaggedForACATS\": false,\n    \"extendedHoursEnrolled\": false,\n    \"lastActivityDate\": \"2024-07-23\",\n    \"interestedParties\": [\n      {\n        \"type\": \"<string>\",\n        \"data\": [\n          {\n            \"id\": {\n              \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n            },\n            \"reportingRole\": \"<string>\",\n            \"tradeDiscretion\": \"<boolean>\",\n            \"from\": \"<dateTime>\",\n            \"to\": \"<dateTime>\",\n            \"endReason\": \"<string>\"\n          },\n          {\n            \"id\": {\n              \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n            },\n            \"reportingRole\": \"<string>\",\n            \"tradeDiscretion\": \"<boolean>\",\n            \"from\": \"<dateTime>\",\n            \"to\": \"<dateTime>\",\n            \"endReason\": \"<string>\"\n          }\n        ]\n      },\n      {\n        \"type\": \"<string>\",\n        \"data\": [\n          {\n            \"id\": {\n              \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n            },\n            \"reportingRole\": \"<string>\",\n            \"tradeDiscretion\": \"<boolean>\",\n            \"from\": \"<dateTime>\",\n            \"to\": \"<dateTime>\",\n            \"endReason\": \"<string>\"\n          },\n          {\n            \"id\": {\n              \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n            },\n            \"reportingRole\": \"<string>\",\n            \"tradeDiscretion\": \"<boolean>\",\n            \"from\": \"<dateTime>\",\n            \"to\": \"<dateTime>\",\n            \"endReason\": \"<string>\"\n          }\n        ]\n      }\n    ]\n  }\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "0f493892-7814-4afb-995a-4dd92d77b3f8",
              "name": "Update Account",
              "request": {
                "name": "Update Account",
                "description": {
                  "content": "Updates an Account details by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "PATCH",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"leverage\": \"<number>\",\n  \"nickname\": \"<string>\",\n  \"status\": \"<string>\",\n  \"accountHolderType\": \"<string>\",\n  \"statusComment\": \"<string>\",\n  \"statusChangeReason\": \"<string>\",\n  \"restricted\": \"<boolean>\",\n  \"ignoreMarketHoursForTest\": \"<boolean>\",\n  \"accountFeatures\": {\n    \"options\": {\n      \"enrolled\": \"<boolean>\",\n      \"optionsLevel\": \"<string>\"\n    },\n    \"mutualFunds\": {\n      \"dividendReinvestment\": \"<boolean>\",\n      \"capitalGainsReinvestment\": \"<boolean>\"\n    },\n    \"fixedIncome\": {\n      \"enrolled\": false\n    },\n    \"equities\": {\n      \"dividendReinvestment\": \"<boolean>\",\n      \"capitalGainsReinvestment\": \"<boolean>\"\n    }\n  },\n  \"authorizedUsers\": [\n    {\n      \"userID\": \"<string>\",\n      \"permissions\": [\n        \"<string>\",\n        \"<string>\"\n      ]\n    },\n    {\n      \"userID\": \"<string>\",\n      \"permissions\": [\n        \"<string>\",\n        \"<string>\"\n      ]\n    }\n  ],\n  \"finra3210ComplianceEntity\": \"<string>\",\n  \"lastActivityDate\": \"<string>\",\n  \"interestedParties\": [\n    {\n      \"type\": \"<string>\",\n      \"data\": [\n        {\n          \"id\": \"<string>\",\n          \"reportingRole\": \"<string>\",\n          \"tradeDiscretion\": \"<boolean>\",\n          \"from\": \"<dateTime>\",\n          \"to\": \"<dateTime>\",\n          \"endReason\": \"<string>\"\n        },\n        {\n          \"id\": \"<string>\",\n          \"reportingRole\": \"<string>\",\n          \"tradeDiscretion\": \"<boolean>\",\n          \"from\": \"<dateTime>\",\n          \"to\": \"<dateTime>\",\n          \"endReason\": \"<string>\"\n        }\n      ]\n    },\n    {\n      \"type\": \"<string>\",\n      \"data\": [\n        {\n          \"id\": \"<string>\",\n          \"reportingRole\": \"<string>\",\n          \"tradeDiscretion\": \"<boolean>\",\n          \"from\": \"<dateTime>\",\n          \"to\": \"<dateTime>\",\n          \"endReason\": \"<string>\"\n        },\n        {\n          \"id\": \"<string>\",\n          \"reportingRole\": \"<string>\",\n          \"tradeDiscretion\": \"<boolean>\",\n          \"from\": \"<dateTime>\",\n          \"to\": \"<dateTime>\",\n          \"endReason\": \"<string>\"\n        }\n      ]\n    }\n  ]\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "36ed6637-1383-4f7b-b2ea-1f6533a25af1",
                  "name": "Updating an Account details by accountID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "PATCH",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"authorizedUsers\": [\n    {\n      \"userID\": \"f6fd0783-2fdb-4ddb-9fd5-2464d8abc267\",\n      \"permissions\": [\n        \"MINOR_GRADUATION_TRANSFER\"\n      ]\n    }\n  ]\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"account\": {\n    \"id\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n    \"accountNo\": \"DWBG000052\",\n    \"accountType\": {\n      \"name\": \"LIVE\",\n      \"description\": \"Live Account\"\n    },\n    \"accountMgmtType\": {\n      \"name\": \"SELF\",\n      \"description\": \"Self Directed Account\"\n    },\n    \"status\": {\n      \"name\": \"OPEN\",\n      \"description\": \"Open\"\n    },\n    \"tradingType\": {\n      \"name\": \"CASH\",\n      \"description\": \"Cash Account\"\n    },\n    \"leverage\": 1,\n    \"nickname\": \"Steve's Robo Advisor Managed Account\",\n    \"parentIB\": {\n      \"id\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9\",\n      \"name\": \"Tendies Trading Company\"\n    },\n    \"taxProfile\": {\n      \"taxStatusCode\": \"W-9\",\n      \"taxRecipientCode\": \"INDIVIDUAL\"\n    },\n    \"commissionID\": \"b3e985dd-9679-63dc-5dd5-9bd7982efecd\",\n    \"beneficiaries\": false,\n    \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n    \"restricted\": false,\n    \"goodFaithViolations\": 0,\n    \"patternDayTrades\": 0,\n    \"freeTradeBalance\": 0,\n    \"gfvPdtExempt\": false,\n    \"buyingPowerOverride\": false,\n    \"bod\": {\n      \"moneyMarket\": 0,\n      \"equityValue\": 0,\n      \"cashAvailableForWithdrawal\": 0,\n      \"cashAvailableForTrading\": 0,\n      \"cashBalance\": 0\n    },\n    \"ria\": {\n      \"advisorID\": \"66304da9-3h6f-2234-935f-ac6b7933d706\",\n      \"productID\": \"product_b94c0b6a-5ac8-43e4-95d1-777051c0503b\"\n    },\n    \"sweepInd\": true,\n    \"interestFree\": false,\n    \"createdWhen\": \"2022-12-22T06:07:41.773Z\",\n    \"openedWhen\": \"2022-12-22T06:07:41Z\",\n    \"updatedWhen\": \"2022-12-11T22:28:21.810Z\",\n    \"ignoreMarketHoursForTest\": false,\n    \"flaggedForACATS\": false,\n    \"extendedHoursEnrolled\": false,\n    \"accountFeatures\": {\n      \"fixedIncome\": {\n        \"enrolled\": true\n      }\n    },\n    \"lastActivityDate\": \"2024-07-23\"\n  }\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "eba9d917-454d-46ea-9db2-438f7a0dc5f5",
              "name": "Retrieve Account Cash",
              "request": {
                "name": "Retrieve Account Cash",
                "description": {
                  "content": "Retrieves an Account Cash details by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "summary",
                    "money"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "e66b387b-55c9-4826-a2c5-b3e510aa29b4",
                  "name": "Retrieving Money details was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "summary",
                        "money"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n  \"accountNo\": \"DWBG000052\",\n  \"tradingType\": \"CASH\",\n  \"updated\": \"2021-04-23T18:41:32.440Z\",\n  \"cash\": {\n    \"cashAvailableForTrade\": 0,\n    \"cashAvailableForWithdrawal\": 0,\n    \"cashBalance\": -12043.23,\n    \"cashSettlement\": [\n      {\n        \"utcTime\": \"2021-04-26T13:30:00.001Z\",\n        \"cash\": 439.7\n      },\n      {\n        \"utcTime\": \"2021-04-26T13:30:00.001Z\",\n        \"cash\": 439.7\n      }\n    ],\n    \"cashPendingSettlement\": 500,\n    \"pendingPaymentsAmount\": 0\n  },\n  \"payments\": {\n    \"buyingPower\": {\n      \"pendingDepositsAmountAvailable\": 20802.71,\n      \"pendingDepositsAmountNotAvailable\": 0\n    },\n    \"redemptions\": {\n      \"amountWithheldFromRedemptions\": 60\n    }\n  }\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "793426a2-11f2-4a30-a2ad-04939f8dfb8c",
              "name": "Retrieve Account Margin",
              "request": {
                "name": "Retrieve Account Margin",
                "description": {
                  "content": "Retrieves Account Margin details by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "summary",
                    "margin"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "1ff3fcc0-eade-4796-8942-1b593e37fb6c",
                  "name": "Retrieving an Account Margin details by accountID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "summary",
                        "margin"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n  \"accountNo\": \"DWBG000052\",\n  \"tradingType\": \"CASH\",\n  \"updated\": \"2017-06-16T15:35:30.617Z\",\n  \"margin\": {\n    \"marginRequirement\": 1,\n    \"longMarketValue\": 0,\n    \"debitBalance\": 0,\n    \"equity\": 0,\n    \"equityFraction\": 0,\n    \"equityRequired\": 1,\n    \"accruedInterest\": 0,\n    \"bodDTBP\": 10000,\n    \"patternDayTrader\": false,\n    \"restricted\": false,\n    \"daySMA\": 0,\n    \"rtExcessEquity\": 0,\n    \"effectiveSMA\": 0,\n    \"noBuyingPowerReason\": \"in officia laborum sit fugiat\",\n    \"marginCall\": {},\n    \"restingOrders\": 0\n  }\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "da5ef928-407b-4570-bf69-f47526ffb7b3",
              "name": "Retrieve Account Lots",
              "request": {
                "name": "Retrieve Account Lots",
                "description": {
                  "content": "Retrieves an Account Lots details by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "position-details"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "24ca69f3-b532-4cd3-a730-fae56af74771",
                  "name": "Retrieving Account Lots details by accountID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "position-details"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"accountID\": \"0d1d686c-abe3-4203-82e5-62f1bd8266f3.1654094651810\",\n  \"accountNo\": \"XYRR000001\",\n  \"positions\": [\n    {\n      \"instrumentID\": \"5b85fabb-d57c-44e6-a7f6-a3efc760226c\",\n      \"symbol\": \"TSLA\",\n      \"currency\": \"USD\",\n      \"costBasis\": 4,\n      \"quantity\": 0.01648699,\n      \"currentMarketPrice\": 253.76,\n      \"currentMarketValue\": 4.18,\n      \"unrealizedPnL\": 0.18,\n      \"effectiveCostPerShare\": 242.6155411,\n      \"side\": \"B\",\n      \"taxLots\": [\n        {\n          \"id\": \"3db27e74626adac3be7b549f2bbc0ab2480852a7\",\n          \"created\": \"2022-08-25T10:07:47.235Z\",\n          \"initialQuantity\": 0.01240767,\n          \"openQuantity\": 0.01240767,\n          \"effectiveCostPerShare\": 241.79,\n          \"side\": \"B\",\n          \"comment\": \"SPLIT CAFB015132 TSLA...\"\n        },\n        {\n          \"id\": \"3db27e74626adac3be7b549f2bbc0ab2480852a7\",\n          \"created\": \"2023-09-25T15:28:12.120Z\",\n          \"initialQuantity\": 0.00407932,\n          \"openQuantity\": 0.00407932,\n          \"effectiveCostPerShare\": 245.14,\n          \"side\": \"B\",\n          \"comment\": \"TSLA FRACK part TSLA KI...\"\n        }\n      ]\n    }\n  ]\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "43790d07-c365-4664-8ed7-5a6883b12244",
              "name": "List User Accounts",
              "request": {
                "name": "List User Accounts",
                "description": {
                  "content": "Retrieves a list of User Accounts by userID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "users",
                    ":userID",
                    "accounts"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) Unique ID of the User to fetch their accounts at DriveWealth.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "userID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "d9d5dda6-600c-4da3-92c2-b05e3bd69ac2",
                  "name": "Retrieving a list of User Accounts by userID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "users",
                        ":userID",
                        "accounts"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) Unique ID of the User to fetch their accounts at DriveWealth.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "userID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"id\": \"8b8ba3fd-74dc-45dc-b2dc-7de683bd713c.1556222995391\",\n    \"accountNo\": \"DWBG000052\",\n    \"nickname\": \"Justin's Self Directed Account\",\n    \"status\": {\n      \"name\": \"PENDING\",\n      \"description\": \"Pending\"\n    },\n    \"accountType\": \"LIVE\",\n    \"accountManagementType\": \"SELF\",\n    \"tradingType\": {\n      \"name\": \"CASH\",\n      \"description\": \"Cash Account\"\n    },\n    \"leverage\": 1,\n    \"commissionID\": \"449d41b9-3940-41ff-b0e6-334adfb443f8\",\n    \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n    \"restricted\": false,\n    \"goodFaithViolations\": 0,\n    \"patternDayTrades\": 0,\n    \"freeTradeBalance\": 0,\n    \"gfvPdtExempt\": false,\n    \"buyingPowerOverride\": false,\n    \"bod\": {\n      \"moneyMarket\": 3028.98,\n      \"equityValue\": 12071.5,\n      \"cashAvailableForWithdrawal\": 3028.98,\n      \"cashAvailableForTrading\": 3028.98,\n      \"updatedWhen\": \"2022-12-12T21:13:12.391Z\"\n    },\n    \"cashBalance\": 3028.98,\n    \"sweepInd\": true,\n    \"interestFree\": false,\n    \"createdWhen\": \"2022-12-11T22:28:21.810Z\",\n    \"updatedWhen\": \"2022-12-11T22:28:21.810Z\",\n    \"lastActivityDate\": \"2024-07-23\",\n    \"interestedParties\": [\n      {\n        \"type\": \"<string>\",\n        \"data\": [\n          {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          }\n        ]\n      },\n      {\n        \"type\": \"<string>\",\n        \"data\": [\n          {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          }\n        ]\n      }\n    ]\n  },\n  {\n    \"id\": \"8b8ba3fd-74dc-45dc-b2dc-7de683bd713c.1556222995391\",\n    \"accountNo\": \"DWBG000052\",\n    \"nickname\": \"Justin's Self Directed Account\",\n    \"status\": {\n      \"name\": \"PENDING\",\n      \"description\": \"Pending\"\n    },\n    \"accountType\": \"LIVE\",\n    \"accountManagementType\": \"SELF\",\n    \"tradingType\": {\n      \"name\": \"CASH\",\n      \"description\": \"Cash Account\"\n    },\n    \"leverage\": 1,\n    \"commissionID\": \"449d41b9-3940-41ff-b0e6-334adfb443f8\",\n    \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n    \"restricted\": false,\n    \"goodFaithViolations\": 0,\n    \"patternDayTrades\": 0,\n    \"freeTradeBalance\": 0,\n    \"gfvPdtExempt\": false,\n    \"buyingPowerOverride\": false,\n    \"bod\": {\n      \"moneyMarket\": 3028.98,\n      \"equityValue\": 12071.5,\n      \"cashAvailableForWithdrawal\": 3028.98,\n      \"cashAvailableForTrading\": 3028.98,\n      \"updatedWhen\": \"2022-12-12T21:13:12.391Z\"\n    },\n    \"cashBalance\": 3028.98,\n    \"sweepInd\": true,\n    \"interestFree\": false,\n    \"createdWhen\": \"2022-12-11T22:28:21.810Z\",\n    \"updatedWhen\": \"2022-12-11T22:28:21.810Z\",\n    \"lastActivityDate\": \"2024-07-23\",\n    \"interestedParties\": [\n      {\n        \"type\": \"<string>\",\n        \"data\": [\n          {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          }\n        ]\n      },\n      {\n        \"type\": \"<string>\",\n        \"data\": [\n          {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          }\n        ]\n      }\n    ]\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "4ab009a1-eadf-415d-8ccc-24bd19349b02",
          "name": "Instruments",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "92981416-e4d5-41d5-9abf-6f157cfb4528",
              "name": "List Instruments",
              "request": {
                "name": "List Instruments",
                "description": {
                  "content": "Retrives a list of Instruments.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "instruments"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "The instrument status; to filter by.",
                        "type": "text/plain"
                      },
                      "key": "status",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The ability to trade options for this instrument; to filter by.",
                        "type": "text/plain"
                      },
                      "key": "isOptionsEnabled",
                      "value": "<boolean>"
                    }
                  ],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "ae3b4d89-a793-40d9-9614-f1100677cbbf",
                  "name": "Retrieving a list of Instruments was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "instruments"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "status",
                          "value": "ACTIVE"
                        },
                        {
                          "key": "isOptionsEnabled",
                          "value": "true"
                        }
                      ],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"id\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n    \"status\": \"ACTIVE\",\n    \"symbol\": \"MS\",\n    \"name\": \"Morgan Stanley\",\n    \"enableExtendedHoursNotionalStatus\": \"INACTIVE\",\n    \"instrumentType\": \"EQUITY\",\n    \"type\": \"EQUITY\",\n    \"ISIN\": \"US023135BX34\",\n    \"isOptionsEnabled\": true,\n    \"CUSIP\": \"E09876AA7\",\n    \"payFrequency\": \"SEMI_ANNUALLY\",\n    \"couponRate\": 0.05,\n    \"maturityDate\": \"2022-05-10\",\n    \"spRating\": \"AAA\",\n    \"bondType\": \"CORPORATE_BOND\",\n    \"domicileCountry\": \"US\"\n  },\n  {\n    \"id\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n    \"status\": \"ACTIVE\",\n    \"symbol\": \"MS\",\n    \"name\": \"Morgan Stanley\",\n    \"enableExtendedHoursNotionalStatus\": \"INACTIVE\",\n    \"instrumentType\": \"EQUITY\",\n    \"type\": \"EQUITY\",\n    \"ISIN\": \"US023135BX34\",\n    \"isOptionsEnabled\": true,\n    \"CUSIP\": \"E09876AA7\",\n    \"payFrequency\": \"SEMI_ANNUALLY\",\n    \"couponRate\": 0.05,\n    \"maturityDate\": \"2022-05-10\",\n    \"spRating\": \"AAA\",\n    \"bondType\": \"CORPORATE_BOND\",\n    \"domicileCountry\": \"US\"\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "bbdab112-11bf-4d87-b01f-615622976038",
              "name": "Retrieve Instrument",
              "request": {
                "name": "Retrieve Instrument",
                "description": {
                  "content": "Retrieves an Instrument details by symbol or instrumentID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "instruments",
                    ":symbolOrInstrumentID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "This query parameter will add an additional property; `fundamentalDataModel` to the response object for an Equity Instrument only. This data consists of financial data model specs for a specific Instrument.",
                        "type": "text/plain"
                      },
                      "key": "options",
                      "value": "<string>"
                    }
                  ],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) A unique ID created by DriveWealth to identify a specific Equity Instrument or Option Instrument, also accept the market symbols like Ticker for Equities and OSI for Options.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "symbolOrInstrumentID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "5604c3b7-f447-4380-9c17-d3c245137d64",
                  "name": "Fetching Instrument details was successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "instruments",
                        ":symbolOrInstrumentID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "options",
                          "value": "Fundamentals"
                        }
                      ],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) A unique ID created by DriveWealth to identify a specific Equity Instrument or Option Instrument, also accept the market symbols like Ticker for Equities and OSI for Options.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "symbolOrInstrumentID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"symbol\": \"MS\",\n  \"name\": \"Morgan Stanley\",\n  \"orderSizeMax\": 20000,\n  \"orderSizeMin\": 0.1,\n  \"orderSizeStep\": 0.01,\n  \"id\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n  \"instrumentType\": \"EQUITY\",\n  \"exchange\": \"NYQ\",\n  \"status\": \"ACTIVE\",\n  \"ISIN\": \"US023135BX34\",\n  \"CUSIP\": \"E09876AA7\",\n  \"settlementDays\": 1,\n  \"reutersPrimaryRic\": \"MS\",\n  \"description\": \"Morgan Stanley is a global financial services company. The Company, through its subsidiaries, provides a range of investment banking, securities, wealth management and investment management services. Its segments include Institutional Securities, Wealth Management and Investment Management. Its Institutional Securities segment provides investment banking, sales and trading, and other services to corporations, governments, financial institutions and high net worth clients. Its Wealth Management segment provides financial services and solutions to individual investors and small-to-medium sized businesses and institutions covering: brokerage and investment advisory services; financial and wealth planning services; workplace services; annuity and insurance products; residential real estate loans and other lending products; banking; and retirement plan services. Its Investment Management segment provides a range of investment strategies and products to a diverse group of clients.\",\n  \"marketTier\": \"Q\",\n  \"sector\": \"Financial Services\",\n  \"industry\": \"Retail (Apparel)\",\n  \"trbc2012\": \"Apparel & Accessories Retailers (NEC)\",\n  \"indexMemberships\": [\n    \"NASDAQ 100 Index\",\n    \"S&P 500\"\n  ],\n  \"incorporatedCountry\": \"USA\",\n  \"isOptionsEnabled\": true,\n  \"longOnly\": true,\n  \"exchangeNickelSpread\": false,\n  \"close\": 87.79,\n  \"enableExtendedHoursNotionalStatus\": \"INACTIVE\",\n  \"fundamentalDataModel\": {\n    \"id\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n    \"symbol\": \"MS\",\n    \"openPrice\": 86.53,\n    \"bidPrice\": 86.12,\n    \"askPrice\": 85.14,\n    \"lowPrice\": 85.83,\n    \"highPrice\": 86.85,\n    \"fiftyTwoWeekLowPrice\": 72.05,\n    \"fiftyTwoWeekHighPrice\": 109.73,\n    \"cumulativeVolume\": 3970567,\n    \"marketCap\": 148374700000,\n    \"peRatio\": 12.7434,\n    \"dividendYield\": 3.5312,\n    \"earningsPerShare\": 6.889,\n    \"dividend\": 3.1,\n    \"sharesOutstanding\": 1307993346,\n    \"timeLastUpdate\": \"18:28:00\",\n    \"bookValuePerShare\": \"59.49634\",\n    \"cashFlowPerShare\": \"10.40132\",\n    \"operatingIncome\": \"19668000000\",\n    \"pbRatio\": \"1.61196\",\n    \"volumeMovingAverage10Day\": 7791905,\n    \"volumeMovingAverage25Day\": 6768708,\n    \"volumeMovingAverage50Day\": 7307176,\n    \"priceMovingAverage50Day\": 85.3034,\n    \"priceMovingAverage150Day\": 83.6295,\n    \"priceMovingAverage200Day\": 84.3036,\n    \"roe\": \"0.15315\",\n    \"percentchangeWTD\": 2.31,\n    \"percentchangeMTD\": 2.3,\n    \"percentchangeYTD\": 10.11,\n    \"percentchange4week\": 21.22,\n    \"percentchange13week\": 6.67,\n    \"percentchange26week\": 8.26,\n    \"percentchange52week\": 12.1,\n    \"percentchange5day\": 10.11,\n    \"percentchangeYTDrelsnp\": 9.11,\n    \"percentchange5weekrelsnp\": 16.62,\n    \"percentchange13weekrelsnp\": 5.67,\n    \"percentchange26weekrelsnp\": 2.66,\n    \"percentchange52weekrelsnp\": 11.12\n  },\n  \"url\": \"http://investor.apple.com\",\n  \"closePrior\": 90.5,\n  \"image\": \"http://syscdn.drivewealth.net/images/symbols/ms.png\",\n  \"isPTP\": false\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "ee698dd6-c332-46e9-a4c1-92591b87242e",
              "name": "Retrieve Instrument Options Chain",
              "request": {
                "name": "Retrieve Instrument Options Chain",
                "description": {
                  "content": "Retrieves an Instrument Options Chain by symbol or instrumentID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "instruments",
                    ":symbolOrInstrumentID",
                    "options"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The expiration date of the option security; to filter by.",
                        "type": "text/plain"
                      },
                      "key": "expirationDate",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "key": "page",
                      "value": "<integer>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The number of option instruments to be returned per page.",
                        "type": "text/plain"
                      },
                      "key": "pageSize",
                      "value": "<integer>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The sorting order of option instruments.",
                        "type": "text/plain"
                      },
                      "key": "sortOrder",
                      "value": "asc"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The number of option instruments to be returned above and below market price.",
                        "type": "text/plain"
                      },
                      "key": "noOfStrikes",
                      "value": "<integer>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The option instruments to be returned above the strike price.",
                        "type": "text/plain"
                      },
                      "key": "minStrikePrice",
                      "value": "<integer>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The option instruments to be returned below the strike price.",
                        "type": "text/plain"
                      },
                      "key": "maxStrikePrice",
                      "value": "<integer>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The type of option instruments to be returned.",
                        "type": "text/plain"
                      },
                      "key": "optionType",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The instrument ID of the option security.",
                        "type": "text/plain"
                      },
                      "key": "id",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The expiration dates for the given underlying security; to filter by.",
                        "type": "text/plain"
                      },
                      "key": "filterBy",
                      "value": "<string>"
                    }
                  ],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) Symbol or instrumentID of the underlying equity security",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "symbolOrInstrumentID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "c1b91606-bceb-42d4-bb28-83d24839eb40",
                  "name": "Retrieving an Instrument Options Chain by symbol or instrumentID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "instruments",
                        ":symbolOrInstrumentID",
                        "options"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "expirationDate",
                          "value": "2022-05-15"
                        },
                        {
                          "key": "page",
                          "value": "1"
                        },
                        {
                          "key": "pageSize",
                          "value": "20"
                        },
                        {
                          "key": "sortOrder",
                          "value": "asc"
                        },
                        {
                          "key": "noOfStrikes",
                          "value": "5"
                        },
                        {
                          "key": "minStrikePrice",
                          "value": "20"
                        },
                        {
                          "key": "maxStrikePrice",
                          "value": "100"
                        },
                        {
                          "key": "optionType",
                          "value": "CALL"
                        },
                        {
                          "key": "id",
                          "value": "3fb1e8a9-f7d5-4d90-95e2-43e7326b5636"
                        },
                        {
                          "key": "filterBy",
                          "value": "expirationDate"
                        }
                      ],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) Symbol or instrumentID of the underlying equity security",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "symbolOrInstrumentID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"symbol\": \"AAPL\",\n  \"options\": [\n    {\n      \"optionsData\": {\n        \"rootSymbol\": \"AAPL\",\n        \"rootId\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n        \"expirationDate\": \"2018-09-18\",\n        \"optionType\": \"PUT\",\n        \"strikePrice\": 16.5,\n        \"deliverable\": 100,\n        \"multiplier\": 100\n      },\n      \"id\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n      \"symbol\": \"AAPL220517P00016000\",\n      \"type\": \"OPTION\",\n      \"name\": \"Apple Computer September 9 $16.00 Put\",\n      \"exchange\": \"NYQ\",\n      \"orderSizeMax\": 20000,\n      \"orderSizeMin\": 1,\n      \"orderSizeStep\": 1\n    }\n  ]\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "bb875037-3804-4986-9f33-a2b9509d51ce",
              "name": "Retrieve Instrument Option Expiration",
              "request": {
                "name": "Retrieve Instrument Option Expiration",
                "description": {
                  "content": "Retrieve an Instrument Option Expiration details by symbol or instrumentID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "instruments",
                    ":symbolOrInstrumentID",
                    "options",
                    "expiration-dates"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) Symbol or instrumentID of the underlying equity security.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "symbolOrInstrumentID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "3029ab2f-c0d1-42d6-8bf5-4d101cf91e9e",
                  "name": "Retrieving an Instrument Option Expiration details by symbol or instrumentID was Successful",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "instruments",
                        ":symbolOrInstrumentID",
                        "options",
                        "expiration-dates"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) Symbol or instrumentID of the underlying equity security.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "symbolOrInstrumentID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"symbol\": \"AAPL\",\n  \"expiration\": [\n    \"2022-05-10\",\n    \"2022-05-11\"\n  ]\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "bf88cc65-9474-4bdc-830a-0b0b3af8d3a7",
              "name": "Search Instruments",
              "request": {
                "name": "Search Instruments",
                "description": {
                  "content": "Searches Instruments based on the filter criteria provided.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "instruments",
                    "filter"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "POST",
                "body": {
                  "mode": "raw",
                  "raw": "[\n  {\n    \"field\": \"<string>\",\n    \"operator\": \"<string>\",\n    \"value1\": \"<string>\",\n    \"value2\": \"<string>\"\n  },\n  {\n    \"field\": \"<string>\",\n    \"operator\": \"<string>\",\n    \"value1\": \"<string>\",\n    \"value2\": \"<string>\"\n  }\n]",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "afa21beb-4a77-493d-88f0-edeb37783683",
                  "name": "Searching Instruments by filter criteria was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "instruments",
                        "filter"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "[\n  {\n    \"field\": \"spRating\",\n    \"operator\": \"><\",\n    \"value1\": \"A\",\n    \"value2\": \"AAA\"\n  }\n]",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"id\": \"2dd415f4-16f0-4df9-9a33-610f1531cb55\",\n    \"name\": \"Amazon.com, Inc. 1.5% 2030-06-03\",\n    \"instrumentType\": \"DEBT\",\n    \"status\": \"ACTIVE\",\n    \"payFrequency\": \"SEMI_ANNUALLY\",\n    \"couponRate\": 1.5,\n    \"maturityDate\": \"2030-06-03\",\n    \"spRating\": \"AA\",\n    \"bondType\": \"CORPORATE_BOND\",\n    \"domicileCountry\": \"US\",\n    \"ISIN\": \"US023135BS49\",\n    \"CUSIP\": \"023135BS4\"\n  },\n  {\n    \"id\": \"f8e3a175-5dfc-4d9b-bd1a-7db0e8b48703\",\n    \"name\": \"Amazon.com, Inc. 3.8% 2024-12-05\",\n    \"instrumentType\": \"DEBT\",\n    \"status\": \"ACTIVE\",\n    \"payFrequency\": \"SEMI_ANNUALLY\",\n    \"couponRate\": 3.8,\n    \"maturityDate\": \"2024-12-05\",\n    \"spRating\": \"AA\",\n    \"bondType\": \"CORPORATE_BOND\",\n    \"domicileCountry\": \"US\",\n    \"ISIN\": \"US023135AN60\",\n    \"CUSIP\": \"023135AN6\"\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "a7013942-8727-42e9-9c17-301a70f5663c",
          "name": "Orders",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "ea08297c-670c-4ddc-afa8-776b0f9589ed",
              "name": "List Account resting Orders",
              "request": {
                "name": "List Account resting Orders",
                "description": {
                  "content": "Retrives a list of Account Orders by accountID. The orders returned will all be currently pending Orders that are awaiting a fill or cancellation.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "summary",
                    "orders"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "05fd6e61-4853-430b-8978-fe04d21a1380",
                  "name": "Retrieving a list of Account Orders was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "summary",
                        "orders"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n  \"accountNo\": \"DWBG000052\",\n  \"tradingType\": \"CASH\",\n  \"updated\": \"2021-04-23T18:41:32.440Z\",\n  \"orders\": [\n    {\n      \"orderID\": \"IC.0e352bb7-9869-4233-9861-9673544efedd\",\n      \"orderNo\": \"ICDU023727\",\n      \"createdWhen\": \"2022-12-11T22:28:21.810Z\",\n      \"symbol\": \"MS\",\n      \"cumQty\": 0.7219,\n      \"orderStatus\": \"2\",\n      \"orderType\": \"1\",\n      \"orderQty\": 0.7219,\n      \"isoTimeRestingOrderExpires\": \"Excepteur voluptate\",\n      \"limitPrice\": -49470468.82257902,\n      \"side\": \"B\",\n      \"orderCashAmt\": -18857827.83251156,\n      \"stopPrice\": 200,\n      \"ISIN\": \"US023135BX34\",\n      \"salesCredit\": {\n        \"currency\": \"USD\",\n        \"amount\": 14\n      },\n      \"instrumentType\": \"EQUITY\"\n    },\n    {\n      \"orderID\": \"IC.0e352bb7-9869-4233-9861-9673544efedd\",\n      \"orderNo\": \"ICDU023727\",\n      \"createdWhen\": \"2022-12-11T22:28:21.810Z\",\n      \"symbol\": \"MS\",\n      \"cumQty\": 0.7219,\n      \"orderStatus\": \"2\",\n      \"orderType\": \"1\",\n      \"orderQty\": 0.7219,\n      \"isoTimeRestingOrderExpires\": \"Lorem anim Excepteur est\",\n      \"limitPrice\": -33118472.778364882,\n      \"side\": \"B\",\n      \"orderCashAmt\": 43119886.0408203,\n      \"stopPrice\": 200,\n      \"ISIN\": \"US023135BX34\",\n      \"salesCredit\": {\n        \"currency\": \"USD\",\n        \"amount\": 14\n      },\n      \"instrumentType\": \"EQUITY\"\n    }\n  ]\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "9f2a51df-759c-49c5-9e51-ff90a8307a12",
              "name": "List Account historical Orders",
              "request": {
                "name": "List Account historical Orders",
                "description": {
                  "content": "Retrieves a list of Account Orders by accountID. The orders returned are ones that have been previously closed, either by being filled or by being canceled.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "reports",
                    "order-history"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) Date start time of data. Follow [ISO 8601 standard](https://en.wikipedia.org/wiki/ISO_8601)",
                        "type": "text/plain"
                      },
                      "key": "from",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) Date end time of data. Follow [ISO 8601 standard](https://en.wikipedia.org/wiki/ISO_8601)",
                        "type": "text/plain"
                      },
                      "key": "to",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The number of orders to be returned per page.",
                        "type": "text/plain"
                      },
                      "key": "limit",
                      "value": "<number>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "Follow [ISO 8601 standard](https://en.wikipedia.org/wiki/ISO_8601)",
                        "type": "text/plain"
                      },
                      "key": "offset",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The direction of pagination.",
                        "type": "text/plain"
                      },
                      "key": "direction",
                      "value": "<string>"
                    }
                  ],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "269b6681-8f3c-4323-9721-18fb8fada71e",
                  "name": "Retrieving a list of Account Orders was Successful",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "reports",
                        "order-history"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "from",
                          "value": "2022-06-16"
                        },
                        {
                          "key": "to",
                          "value": "2022-07-16"
                        },
                        {
                          "key": "limit",
                          "value": "25"
                        },
                        {
                          "key": "offset",
                          "value": "2022-07-16"
                        },
                        {
                          "key": "direction",
                          "value": "prev"
                        }
                      ],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n  \"accountNo\": \"DWBG000052\",\n  \"tradingType\": \"CASH\",\n  \"updated\": \"2017-06-16T15:35:30.617Z\",\n  \"orders\": [\n    {\n      \"orderID\": \"IC.0e352bb7-9869-4233-9861-9673544efedd\",\n      \"orderNo\": \"ICDU023727\",\n      \"createdWhen\": \"2022-12-11T22:28:21.810Z\",\n      \"symbol\": \"MS\",\n      \"cumQty\": 0.7219,\n      \"orderStatus\": 2,\n      \"orderType\": \"MARKET\",\n      \"orderQty\": 0.7219,\n      \"isoTimeRestingOrderExpires\": \"quis eu occaecat\",\n      \"limitPrice\": -44956732.26138233,\n      \"side\": \"B\",\n      \"mitTriggerPrice\": 0,\n      \"triggered\": 0,\n      \"averagePriceRaw\": 147.45,\n      \"orderCashAmt\": 92850205.3971011,\n      \"stopPrice\": 200,\n      \"ISIN\": \"US023135BX34\"\n    },\n    {\n      \"orderID\": \"IC.0e352bb7-9869-4233-9861-9673544efedd\",\n      \"orderNo\": \"ICDU023727\",\n      \"createdWhen\": \"2022-12-11T22:28:21.810Z\",\n      \"symbol\": \"MS\",\n      \"cumQty\": 0.7219,\n      \"orderStatus\": 2,\n      \"orderType\": \"MARKET\",\n      \"orderQty\": 0.7219,\n      \"isoTimeRestingOrderExpires\": \"ut do aliquip\",\n      \"limitPrice\": -64811958.76867365,\n      \"side\": \"B\",\n      \"mitTriggerPrice\": 0,\n      \"triggered\": 0,\n      \"averagePriceRaw\": 147.45,\n      \"orderCashAmt\": -58953948.767643236,\n      \"stopPrice\": 200,\n      \"ISIN\": \"US023135BX34\"\n    }\n  ]\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "903c96fb-adc3-4035-b349-f99c85f14208",
              "name": "Create Order",
              "request": {
                "name": "Create Order",
                "description": {
                  "content": "Create an Order.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "orders"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "POST",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"accountNo\": \"<string>\",\n  \"orderType\": \"<string>\",\n  \"side\": \"<string>\",\n  \"limitType\": \"<string>\",\n  \"symbol\": \"<string>\",\n  \"instrumentID\": \"<uuid>\",\n  \"ISIN\": \"<string>\",\n  \"quantity\": \"<double>\",\n  \"amountCash\": \"<double>\",\n  \"price\": \"<double>\",\n  \"currency\": \"<string>\",\n  \"commission\": \"<double>\",\n  \"commissionRate\": \"<BigDecimal>\",\n  \"clientNotes\": \"<string>\",\n  \"preventQueuing\": \"<boolean>\",\n  \"extendedHours\": \"<boolean>\",\n  \"metadata\": \"<object>\",\n  \"timeInForce\": \"<string>\",\n  \"expiration\": \"<date>\",\n  \"salesCredit\": {\n    \"currency\": \"<string>\",\n    \"amount\": \"<integer>\"\n  },\n  \"dccs\": \"<boolean>\",\n  \"taxLotDisposition\": [\n    {\n      \"taxLotID\": \"<string>\"\n    },\n    {\n      \"taxLotID\": \"<string>\"\n    }\n  ],\n  \"travelRuleBankAccountID\": \"<string>\",\n  \"traderID\": \"<string>\",\n  \"clientOrderTransactionTime\": \"<string>\",\n  \"clientOrderID\": \"<string>\",\n  \"deptType\": \"<string>\"\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "6f805daf-a5e4-45a1-9958-cc62f3fbab96",
                  "name": "Creating an Order was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "orders"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"accountNo\": \"DWFS001102\",\n  \"orderType\": \"MARKET\",\n  \"symbol\": \"SBUX\",\n  \"side\": \"BUY\",\n  \"amountCash\": 100\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"orderId\": \"EF.418a5506-256c-4c3c-9d4d-f491522cf7f2\",\n  \"orderNo\": \"EFXM000103\"\n}",
                  "cookie": []
                },
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "0addee69-844a-4245-bdce-6612d410c038",
                  "name": "Bad Request",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "orders"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"accountNo\": \"DWFS001102\",\n  \"orderType\": \"MARKET\",\n  \"symbol\": \"SBUX\",\n  \"side\": \"BUY\",\n  \"amountCash\": 100\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "Bad Request",
                  "code": 400,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"errorCode\": \"E032\",\n  \"message\": \"Invalid or missing parameters in the request body. Refer to the API documentation for details.\",\n  \"errorDetails\": {\n    \"detail\": \"Cannot specify both 'commission' and 'commissionRate'. Provide either 'commission' or 'commissionRate'\",\n    \"field\": \"commission/commissionRate\",\n    \"type\": \"DECIMAL\"\n  }\n}",
                  "cookie": []
                },
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "1368af43-8c8b-4b66-9545-0d6601ad3e0f",
                  "name": "Account restricted to make day trades",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "orders"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"accountNo\": \"DWFS001102\",\n  \"orderType\": \"MARKET\",\n  \"symbol\": \"SBUX\",\n  \"side\": \"BUY\",\n  \"amountCash\": 100\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "Forbidden",
                  "code": 403,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"errorCode\": \"A051\",\n  \"message\": \"Account has been restricted. Check account status and notes for details. Forbidden: Account is restricted from making day trades. accountID=<accountID>\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "a8af944e-2c0f-463c-9180-80ad98d8affd",
              "name": "Retrieve Order",
              "request": {
                "name": "Retrieve Order",
                "description": {
                  "content": "Retrieves an Order details by orderID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "orders",
                    ":orderID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "orderID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "147b542a-78b6-40c4-a0a7-a3be06d475da",
                  "name": "Fetching Order status was successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "orders",
                        ":orderID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "orderID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"EF.418a5506-256c-4c3c-9d4d-f491522cf7f2\",\n  \"orderNo\": \"EFXM000103\",\n  \"type\": \"MARKET\",\n  \"side\": {},\n  \"status\": \"FILLED\",\n  \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n  \"ISIN\": \"US023135BX34\",\n  \"CUSIP\": \"E09876AA7\",\n  \"symbol\": \"MS\",\n  \"averagePrice\": 160,\n  \"currency\": \"USD\",\n  \"totalOrderAmount\": 800,\n  \"cumulativeQuantity\": 5,\n  \"quantity\": 5,\n  \"fees\": 0.01,\n  \"ptpWithholdingFee\": 0.01,\n  \"createdBy\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n  \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n  \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407776996299\",\n  \"accountNo\": \"CSSW000001\",\n  \"created\": \"2019-02-14T18:56:07.411Z\",\n  \"statusMessage\": {\n    \"errorCode\": {},\n    \"message\": \"ut laboris ullamco sunt\",\n    \"reason\": \"et ut mollit sunt\"\n  },\n  \"amountCash\": 800,\n  \"OrderExpires\": \"sunt Lorem\",\n  \"salesCredit\": {\n    \"currency\": \"USD\",\n    \"amount\": 14\n  },\n  \"instrumentType\": \"EQUITY\",\n  \"dccs\": true,\n  \"openQuantity\": 1,\n  \"availableForTradingQuantity\": 1,\n  \"travelRuleBankAccountID\": \"bank_485ba18c-009d-4c4a-a6e9-99b104c800b2\",\n  \"clientOrderTransactionTime\": \"2024-07-30T22:13:18.000Z\",\n  \"clientOrderID\": \"5a1762d5-4562\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "d9ec5745-973f-402c-85bd-f6847220416a",
              "name": "Update Order",
              "request": {
                "name": "Update Order",
                "description": {
                  "content": "Updates an Order by orderID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "orders",
                    ":orderID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "orderID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "PATCH",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"method\": \"<string>\",\n  \"traderID\": \"<string>\",\n  \"clientOrderTransactionTime\": \"<string>\",\n  \"clientOrderID\": \"<string>\"\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "cab5c729-5b9b-4837-b2ee-5f35209cb2fc",
                  "name": "The Order was Successfully Updated.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "orders",
                        ":orderID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "orderID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "PATCH",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"method\": \"CANCEL\",\n  \"traderID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n  \"clientOrderTransactionTime\": \"2024-07-30T22:13:18.000Z\",\n  \"clientOrderID\": \"5a1762d5-4562\"\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"orderId\": \"EF.418a5506-256c-4c3c-9d4d-f491522cf7f2\",\n  \"orderNo\": \"EFXM000103\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "ce51c35b-19db-4fa8-a497-47685b2227b8",
              "name": "Retrieve Order by Order Number",
              "request": {
                "name": "Retrieve Order by Order Number",
                "description": {
                  "content": "Retrieves an Order by OrderNo.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "orders",
                    "byOrderNo",
                    ":orderNo"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "orderNo"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "6b6d9588-531a-4284-98c8-90e53618533e",
                  "name": " Retrieving an Order by OrderNo was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "orders",
                        "byOrderNo",
                        ":orderNo"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "orderNo"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"EF.418a5506-256c-4c3c-9d4d-f491522cf7f2\",\n  \"orderNo\": \"EFXM000103\",\n  \"type\": \"MARKET\",\n  \"side\": {},\n  \"status\": \"FILLED\",\n  \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n  \"ISIN\": \"US023135BX34\",\n  \"CUSIP\": \"E09876AA7\",\n  \"symbol\": \"MS\",\n  \"averagePrice\": 160,\n  \"currency\": \"USD\",\n  \"totalOrderAmount\": 800,\n  \"cumulativeQuantity\": 5,\n  \"quantity\": 5,\n  \"fees\": 0.01,\n  \"ptpWithholdingFee\": 0.01,\n  \"createdBy\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n  \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n  \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407776996299\",\n  \"accountNo\": \"CSSW000001\",\n  \"created\": \"2019-02-14T18:56:07.411Z\",\n  \"statusMessage\": {\n    \"errorCode\": {},\n    \"message\": \"ut laboris ullamco sunt\",\n    \"reason\": \"et ut mollit sunt\"\n  },\n  \"amountCash\": 800,\n  \"OrderExpires\": \"sunt Lorem\",\n  \"salesCredit\": {\n    \"currency\": \"USD\",\n    \"amount\": 14\n  },\n  \"instrumentType\": \"EQUITY\",\n  \"dccs\": true,\n  \"openQuantity\": 1,\n  \"availableForTradingQuantity\": 1,\n  \"travelRuleBankAccountID\": \"bank_485ba18c-009d-4c4a-a6e9-99b104c800b2\",\n  \"clientOrderTransactionTime\": \"2024-07-30T22:13:18.000Z\",\n  \"clientOrderID\": \"5a1762d5-4562\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "377d87eb-0e1b-46c8-b1a1-c45f49225a87",
          "name": "Positions",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "b287c9cd-ad15-41b2-ae32-7cadde98badd",
              "name": "List Account Positions",
              "request": {
                "name": "List Account Positions",
                "description": {
                  "content": "Retrives a list of Account Positions by accountID",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "summary",
                    "positions"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "f95f3712-a2d7-40de-87ce-40e572d1f8cd",
                  "name": "Retrieving an Account's Positions by accountID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "summary",
                        "positions"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n  \"accountNo\": \"DWBG000052\",\n  \"tradingType\": \"CASH\",\n  \"updated\": \"2017-06-16T15:35:30.617Z\",\n  \"equityValue\": 34275565.44,\n  \"optionsValue\": 12345.67,\n  \"debtValue\": 12345.67,\n  \"positionsValue\": 34287911.11,\n  \"equityPositions\": [\n    {\n      \"symbol\": \"MS\",\n      \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n      \"ISIN\": \"US023135BX34\",\n      \"instrumentType\": \"EQUITY\",\n      \"openQty\": 31.65120151,\n      \"costBasis\": 975.98,\n      \"marketValue\": 4540.36,\n      \"side\": \"B\",\n      \"priorClose\": 144.29,\n      \"availableForTradingQty\": 31.65120151,\n      \"avgPrice\": 30.84,\n      \"mktPrice\": 143.45,\n      \"unrealizedPL\": 3564.38,\n      \"unrealizedDayPLPercent\": -0.58,\n      \"unrealizedDayPL\": -26.59\n    },\n    {\n      \"symbol\": \"MS\",\n      \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n      \"ISIN\": \"US023135BX34\",\n      \"instrumentType\": \"EQUITY\",\n      \"openQty\": 31.65120151,\n      \"costBasis\": 975.98,\n      \"marketValue\": 4540.36,\n      \"side\": \"B\",\n      \"priorClose\": 144.29,\n      \"availableForTradingQty\": 31.65120151,\n      \"avgPrice\": 30.84,\n      \"mktPrice\": 143.45,\n      \"unrealizedPL\": 3564.38,\n      \"unrealizedDayPLPercent\": -0.58,\n      \"unrealizedDayPL\": -26.59\n    }\n  ],\n  \"optionsPositions\": [\n    {\n      \"symbol\": \"MS\",\n      \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n      \"ISIN\": \"US023135BX34\",\n      \"instrumentType\": \"EQUITY\",\n      \"openQty\": 31.65120151,\n      \"costBasis\": 975.98,\n      \"marketValue\": 4540.36,\n      \"side\": \"B\",\n      \"priorClose\": 144.29,\n      \"availableForTradingQty\": 31.65120151,\n      \"avgPrice\": 30.84,\n      \"mktPrice\": 440.75,\n      \"unrealizedPL\": 14.24,\n      \"unrealizedDayPLPercent\": 1.65,\n      \"unrealizedDayPL\": 0.54\n    },\n    {\n      \"symbol\": \"MS\",\n      \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n      \"ISIN\": \"US023135BX34\",\n      \"instrumentType\": \"EQUITY\",\n      \"openQty\": 31.65120151,\n      \"costBasis\": 975.98,\n      \"marketValue\": 4540.36,\n      \"side\": \"B\",\n      \"priorClose\": 144.29,\n      \"availableForTradingQty\": 31.65120151,\n      \"avgPrice\": 30.84,\n      \"mktPrice\": 440.75,\n      \"unrealizedPL\": 14.24,\n      \"unrealizedDayPLPercent\": 1.65,\n      \"unrealizedDayPL\": 0.54\n    }\n  ],\n  \"mutualFundsPositions\": [\n    {\n      \"symbol\": \"MS\",\n      \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n      \"ISIN\": \"US023135BX34\",\n      \"instrumentType\": \"EQUITY\",\n      \"openQty\": 31.65120151,\n      \"costBasis\": 975.98,\n      \"marketValue\": 4540.36,\n      \"side\": \"B\",\n      \"priorClose\": 144.29,\n      \"availableForTradingQty\": 31.65120151,\n      \"avgPrice\": 30.84\n    },\n    {\n      \"symbol\": \"MS\",\n      \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n      \"ISIN\": \"US023135BX34\",\n      \"instrumentType\": \"EQUITY\",\n      \"openQty\": 31.65120151,\n      \"costBasis\": 975.98,\n      \"marketValue\": 4540.36,\n      \"side\": \"B\",\n      \"priorClose\": 144.29,\n      \"availableForTradingQty\": 31.65120151,\n      \"avgPrice\": 30.84\n    }\n  ],\n  \"debtPositions\": [\n    {\n      \"symbol\": \"MS\",\n      \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n      \"ISIN\": \"US023135BX34\",\n      \"instrumentType\": \"EQUITY\",\n      \"openQty\": 31.65120151,\n      \"costBasis\": 975.98,\n      \"marketValue\": 4540.36,\n      \"side\": \"B\",\n      \"priorClose\": 144.29,\n      \"availableForTradingQty\": 31.65120151,\n      \"avgPrice\": 30.84\n    },\n    {\n      \"symbol\": \"MS\",\n      \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n      \"ISIN\": \"US023135BX34\",\n      \"instrumentType\": \"EQUITY\",\n      \"openQty\": 31.65120151,\n      \"costBasis\": 975.98,\n      \"marketValue\": 4540.36,\n      \"side\": \"B\",\n      \"priorClose\": 144.29,\n      \"availableForTradingQty\": 31.65120151,\n      \"avgPrice\": 30.84\n    }\n  ]\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "6bf01e43-c166-415a-ae28-50c70587e18b",
              "name": "Retrieve Account Option Positions",
              "request": {
                "name": "Retrieve Account Option Positions",
                "description": {
                  "content": "Retrieves Account Option Positions",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "options",
                    "positions"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "The expiration date of options; to filter by.",
                        "type": "text/plain"
                      },
                      "key": "filterBy",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The start date of the range of option's expiration.",
                        "type": "text/plain"
                      },
                      "key": "from",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The end date of the range of option's expiration.",
                        "type": "text/plain"
                      },
                      "key": "to",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The number of results to be returned.",
                        "type": "text/plain"
                      },
                      "key": "limit",
                      "value": "50"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The identifier of the page.",
                        "type": "text/plain"
                      },
                      "key": "offset",
                      "value": "<string>"
                    }
                  ],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "17467986-9135-4cf8-9f81-77bb37872895",
                  "name": "Retrieving Account Option Positions was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "options",
                        "positions"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "filterBy",
                          "value": "expirationDate"
                        },
                        {
                          "key": "from",
                          "value": "2023-02-16"
                        },
                        {
                          "key": "to",
                          "value": "2023-02-16"
                        },
                        {
                          "key": "limit",
                          "value": "10"
                        },
                        {
                          "key": "offset",
                          "value": "86572e14-84ae-4f0c-9533-3c9432637f8e.1627500314555#65d1aee9-9a6c-4720-9879-71c4fcf43060.2023-12-07T21:17:45.743Z"
                        }
                      ],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"data\": [\n    {\n      \"expirationDate\": \"2018-09-18\",\n      \"position\": {\n        \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n        \"accountNo\": \"DWBG000052\",\n        \"costBasis\": 975.98,\n        \"effectivePx\": 975.98,\n        \"execID\": \"170638430890297892000\",\n        \"initPx\": 975.98,\n        \"initQty\": 0.01,\n        \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n        \"side\": \"B\",\n        \"openQty\": 10,\n        \"comment\": \"TOP\"\n      },\n      \"instrument\": {\n        \"rootSymbol\": \"AAPL\",\n        \"rootId\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n        \"symbol\": \"MS\",\n        \"optionType\": \"PUT\",\n        \"marketPrice\": 16.5,\n        \"strikePrice\": 16.5\n      }\n    },\n    {\n      \"expirationDate\": \"2018-09-18\",\n      \"position\": {\n        \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n        \"accountNo\": \"DWBG000052\",\n        \"costBasis\": 975.98,\n        \"effectivePx\": 975.98,\n        \"execID\": \"170638430890297892000\",\n        \"initPx\": 975.98,\n        \"initQty\": 0.01,\n        \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n        \"side\": \"B\",\n        \"openQty\": 10,\n        \"comment\": \"TOP\"\n      },\n      \"instrument\": {\n        \"rootSymbol\": \"AAPL\",\n        \"rootId\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n        \"symbol\": \"MS\",\n        \"optionType\": \"PUT\",\n        \"marketPrice\": 16.5,\n        \"strikePrice\": 16.5\n      }\n    }\n  ],\n  \"nextPageOffset\": \"86572e14-84ae-4f0c-9533-3c9432637f8e.1627500314555#65d1aee9-9a6c-4720-9879-71c4fcf43060.2023-12-07T21:17:45.743Z\",\n  \"prevPageOffset\": \"86572e14-84ae-4f0c-9533-3c9432637f8e.1627500314555#65d1aee9-9a6c-4720-9879-71c4fcf43060.2023-12-07T21:17:45.743Z\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "7dd0ca5e-e718-4c05-8578-ec15ed36286f",
          "name": "Transactions",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "ef02a57e-aa70-4219-91af-4e3620fec1be",
              "name": "List Account Transactions",
              "request": {
                "name": "List Account Transactions",
                "description": {
                  "content": "Retrieves a list of Account Transactions by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "transactions"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) Date start time of data. Follow [ISO 8601 standard](https://en.wikipedia.org/wiki/ISO_8601)",
                        "type": "text/plain"
                      },
                      "key": "from",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) Date end time of data. Follow [ISO 8601 standard](https://en.wikipedia.org/wiki/ISO_8601)",
                        "type": "text/plain"
                      },
                      "key": "to",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The number of transactions to be returned per page.",
                        "type": "text/plain"
                      },
                      "key": "limit",
                      "value": "<number>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "Follow [ISO 8601 standard](https://en.wikipedia.org/wiki/ISO_8601)",
                        "type": "text/plain"
                      },
                      "key": "offset",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The direction of pagination",
                        "type": "text/plain"
                      },
                      "key": "direction",
                      "value": "<string>"
                    }
                  ],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "fa8daf5d-2435-4907-beb5-05be7f823717",
                  "name": "Retrieving a list of Account Transactions was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "transactions"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "from",
                          "value": "2022-06-16"
                        },
                        {
                          "key": "to",
                          "value": "2022-07-16"
                        },
                        {
                          "key": "limit",
                          "value": "25"
                        },
                        {
                          "key": "offset",
                          "value": "2022-07-16"
                        },
                        {
                          "key": "direction",
                          "value": "prev"
                        }
                      ],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"accountAmount\": -890.12,\n    \"accountBalance\": 49984.44,\n    \"accountType\": \"LIVE\",\n    \"dividend\": {\n      \"type\": \"CASH\",\n      \"amountPerShare\": 0.65,\n      \"taxCode\": \"FULLY_TAXABLE\"\n    },\n    \"dividendTax\": {\n      \"rate\": 0.15,\n      \"type\": \"FOREIGN_TAX\"\n    },\n    \"dnb\": false,\n    \"comment\": \"Buy 0.0259 shares of AMZN at 1003.13 FULL fill\",\n    \"finTranID\": \"EF.a935f686-5567-4e10-9e71-261314207c0b\",\n    \"finTranTypeID\": \"JNLC\",\n    \"feeSec\": 0.01,\n    \"feeTaf\": 0.01,\n    \"feeBase\": 0.02,\n    \"feeXtraShares\": 0.05,\n    \"feeExchange\": 0.02,\n    \"fillQty\": 1.02387115,\n    \"fillPx\": 17.44,\n    \"orderID\": \"IC.0e352bb7-9869-4233-9861-9673544efedd\",\n    \"mergerAcquisition\": {\n      \"type\": \"ADD_SHARES_CASH\",\n      \"acquirer\": {\n        \"id\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n        \"symbol\": \"AAPL\",\n        \"name\": \"Apple\"\n      },\n      \"acquiree\": {\n        \"id\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n        \"symbol\": \"TSLA\",\n        \"name\": \"TSLA\"\n      }\n    },\n    \"positionDelta\": 0.18\n  },\n  {\n    \"accountAmount\": -890.12,\n    \"accountBalance\": 49984.44,\n    \"accountType\": \"LIVE\",\n    \"dividend\": {\n      \"type\": \"CASH\",\n      \"amountPerShare\": 0.65,\n      \"taxCode\": \"FULLY_TAXABLE\"\n    },\n    \"dividendTax\": {\n      \"rate\": 0.15,\n      \"type\": \"FOREIGN_TAX\"\n    },\n    \"dnb\": false,\n    \"comment\": \"Buy 0.0259 shares of AMZN at 1003.13 FULL fill\",\n    \"finTranID\": \"EF.a935f686-5567-4e10-9e71-261314207c0b\",\n    \"finTranTypeID\": \"JNLC\",\n    \"feeSec\": 0.01,\n    \"feeTaf\": 0.01,\n    \"feeBase\": 0.02,\n    \"feeXtraShares\": 0.05,\n    \"feeExchange\": 0.02,\n    \"fillQty\": 1.02387115,\n    \"fillPx\": 17.44,\n    \"orderID\": \"IC.0e352bb7-9869-4233-9861-9673544efedd\",\n    \"mergerAcquisition\": {\n      \"type\": \"REMOVE_SHARES\",\n      \"acquirer\": {\n        \"id\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n        \"symbol\": \"AAPL\",\n        \"name\": \"Apple\"\n      },\n      \"acquiree\": {\n        \"id\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n        \"symbol\": \"TSLA\",\n        \"name\": \"TSLA\"\n      }\n    },\n    \"positionDelta\": 0.18\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "f4c77ad1-9366-4865-adfa-a060579a5368",
          "name": "Exchanges",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "eb932f1b-a160-4278-bd9a-4051902045c8",
              "name": "Create Instrument Exchange",
              "request": {
                "name": "Create Instrument Exchange",
                "description": {
                  "content": "Creates an Instrument Exchange. The ability to sale of a held instrument and purchase of another.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "exchanges"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "POST",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"accountNo\": \"<string>\",\n  \"sellSymbol\": \"<string>\",\n  \"buySymbol\": \"<string>\",\n  \"amountCash\": \"<number>\",\n  \"quantity\": \"<number>\"\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "b4539e0b-ec49-44a1-b5f9-d585a27f812f",
                  "name": "Creating an Exchange was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "exchanges"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"accountNo\": \"DWPH000003\",\n  \"sellSymbol\": \"VTSMX\",\n  \"buySymbol\": \"VTSAX\",\n  \"amountCash\": 100,\n  \"quantity\": 10\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"IC.0e352bb7-9869-4233-9861-1173544efedd\",\n  \"exchangeNo\": \"ICDU023727\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "03b0e013-38d4-46d8-9c85-20607e2a48b0",
              "name": "Update Instrument Exchange",
              "request": {
                "name": "Update Instrument Exchange",
                "description": {
                  "content": "Updates an Instrument Exchange.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "exchanges"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "PATCH",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"method\": \"<string>\"\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "b6bc33bb-98ff-4152-94fe-aa1f15504562",
                  "name": "OK",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "exchanges"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "PATCH",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"method\": \"CANCEL\"\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"IC.0e352bb7-9869-4233-9861-1173544efedd\",\n  \"exchangeNo\": \"ICDU023727\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "b784f15c-fd0f-49b0-ab1d-35b0191b0a78",
              "name": "Retrieve Exchange",
              "request": {
                "name": "Retrieve Exchange",
                "description": {
                  "content": "To retrieve specific exchange details the exchange endpoint can be used. In addition the underlying buy and sell trades, which make up the exchange order, will be available through the existing get order endpoint. ",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "exchanges",
                    ":exchangeIdentifier"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The Exchange ID (id) or Exchange Number (exchangeNo)",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "exchangeIdentifier"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "eab2da53-c80c-4727-a91b-2da2aef0c909",
                  "name": "OK",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "exchanges",
                        ":exchangeIdentifier"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) The Exchange ID (id) or Exchange Number (exchangeNo)",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "exchangeIdentifier"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"GC.f7590a52-75c7-4f3a-92c7-6b03e02dc44f\",\n  \"exchangeNo\": \"ICDU023727\",\n  \"status\": \"FILLED\",\n  \"sellSymbol\": \"VTSMX\",\n  \"sellOrderId\": \"GC.f7590a52-75c7-4f3a-92c7-6b03e02d111\",\n  \"sellOrderNo\": \"EFXM000103\",\n  \"buySymbol\": \"VTSAX\",\n  \"buyOrderId\": \"GC.f7590a52-75c7-4f3a-92c7-6b03e02d222\",\n  \"buyOrderNo\": \"EFXM001102\",\n  \"sellAveragePrice\": 10,\n  \"sellCumulativeQuantity\": 100,\n  \"buyAveragePrice\": 50,\n  \"buyCumulativeQuantity\": 20,\n  \"amountCash\": 1000,\n  \"fees\": 0,\n  \"orderExpires\": \"2019-03-29T20:00:00.000Z\",\n  \"createdBy\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd\",\n  \"userID\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd\",\n  \"accountID\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd.1403540676095\",\n  \"accountNo\": \"DWZR000001\",\n  \"created\": \"2019-03-28T22:40:03.240Z\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "2be1ba1b-4fdd-4b12-b7c3-a4b3871b8f62",
              "name": "List Account Instrument Exchanges.",
              "request": {
                "name": "List Account Instrument Exchanges.",
                "description": {
                  "content": "Retrives a list of Account Instrument Exchanges by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "summary",
                    "exchanges"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The account id of the user where the order was placed",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "9c549b8a-e8f5-49fa-adb8-6b0f17b574af",
                  "name": "Retrieving a list of Account Instrument Exchanges by accountID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "summary",
                        "exchanges"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) The account id of the user where the order was placed",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"accountID\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd.1403540676095\",\n  \"accountNo\": \"DWBG000052\",\n  \"tradingType\": \"CASH\",\n  \"updated\": \"2021-04-23T18:41:32.440Z\",\n  \"exchanges\": [\n    {\n      \"id\": \"GC.f7590a52-75c7-4f3a-92c7-6b03e02dc11f\",\n      \"exchangeNo\": \"ICDU023727\",\n      \"status\": \"NEW\",\n      \"sellSymbol\": \"VTSMX\",\n      \"sellOrderId\": \"GC.f7590a52-75c7-4f3a-92c7-6b03e02d112\",\n      \"sellOrderNo\": \"EFXM000203\",\n      \"buySymbol\": \"VTSAX\",\n      \"buyOrderId\": \"GC.f7590a52-75c7-4f3a-92c7-6b03e02d223\",\n      \"buyOrderNo\": \"EFXM002102\",\n      \"amountCash\": 0,\n      \"sellAveragePrice\": 0,\n      \"sellCumulativeQuantity\": 0,\n      \"buyAveragePrice\": 0,\n      \"buyCumulativeQuantity\": 0,\n      \"fees\": 0,\n      \"orderExpires\": \"2019-03-29T20:00:00.000Z\",\n      \"createdBy\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd\",\n      \"userID\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd\",\n      \"accountID\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd.1403540676095\",\n      \"accountNo\": \"DWZR000001\",\n      \"created\": \"2019-03-28T22:40:03.240Z\"\n    }\n  ]\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "7167211d-506c-40d2-8f6e-042e52a01e76",
              "name": "Retrieve Account Instrument Exchange History",
              "request": {
                "name": "Retrieve Account Instrument Exchange History",
                "description": {
                  "content": "Retrieves a list of Account Instrument Exchange History by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "reports",
                    "exchange-history"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The account id of the user where the order was placed",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "890b8508-2863-4e45-8d64-05e31da9fd1d",
                  "name": "Retrieving Account Instrument Exchange History was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "reports",
                        "exchange-history"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) The account id of the user where the order was placed",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"accountID\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd.1403540676095\",\n  \"accountNo\": \"DWBG000052\",\n  \"tradingType\": \"CASH\",\n  \"updated\": \"2021-04-23T18:41:32.440Z\",\n  \"exchanges\": [\n    {\n      \"id\": \"GC.f7590a52-75c7-4f3a-92c7-6b03e02dc11f\",\n      \"exchangeNo\": \"ICDU023727\",\n      \"status\": \"FILLED\",\n      \"sellSymbol\": \"VTSMX\",\n      \"sellOrderId\": \"GC.f7590a52-75c7-4f3a-92c7-6b03e02d112\",\n      \"sellOrderNo\": \"EFXM000203\",\n      \"buySymbol\": \"VTSAX\",\n      \"buyOrderId\": \"GC.f7590a52-75c7-4f3a-92c7-6b03e02d223\",\n      \"buyOrderNo\": \"EFXM002102\",\n      \"amountCash\": 1000,\n      \"sellAveragePrice\": 10,\n      \"sellCumulativeQuantity\": 100,\n      \"buyAveragePrice\": 50,\n      \"buyCumulativeQuantity\": 20,\n      \"fees\": 0,\n      \"orderExpires\": \"2019-03-29T20:00:00.000Z\",\n      \"createdBy\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd\",\n      \"userID\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd\",\n      \"accountID\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd.1403540676095\",\n      \"accountNo\": \"DWZR000001\",\n      \"created\": \"2019-03-28T22:40:03.240Z\"\n    }\n  ]\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "6d169bd4-21f0-4f07-a4a2-d2041cd9645c",
          "name": "Commission Schedules",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "1bac287d-f5b4-420c-b2d8-bd0ac93235cb",
              "name": "List Commission Schedules",
              "request": {
                "name": "List Commission Schedules",
                "description": {
                  "content": "Retrieves a list of Commissions Schedules by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "commissions"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "5a812174-91d7-410e-9dfd-abd32f644f06",
                  "name": "Retrieving a list of Commissions Schedules was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "commissions"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"active\": true,\n    \"commissionID\": \"b3e985dd-9679-63dc-5dd5-9bd7982efecd\",\n    \"description\": \"Free\",\n    \"assignmentCriteria\": {\n      \"wplID\": \"TTC\",\n      \"countries\": \"USA\",\n      \"defaultStatus\": true,\n      \"accountMgmtType\": \"voluptate amet minim\"\n    },\n    \"rates\": {\n      \"fractional\": {\n        \"schema\": {\n          \"rate\": 1.49,\n          \"passThroughFees\": true,\n          \"shareAmountRounding\": \"CEIL\",\n          \"minimumRate\": 1.49\n        }\n      },\n      \"default\": {\n        \"schema\": {\n          \"rate\": 1.49,\n          \"passThroughFees\": true,\n          \"shareAmountRounding\": \"CEIL\",\n          \"minimumRate\": 1.49\n        }\n      }\n    }\n  },\n  {\n    \"active\": true,\n    \"commissionID\": \"b3e985dd-9679-63dc-5dd5-9bd7982efecd\",\n    \"description\": \"Free\",\n    \"assignmentCriteria\": {\n      \"wplID\": \"TTC\",\n      \"countries\": \"USA\",\n      \"defaultStatus\": true,\n      \"accountMgmtType\": \"sint aute ut\"\n    },\n    \"rates\": {\n      \"fractional\": {\n        \"schema\": {\n          \"rate\": 1.49,\n          \"passThroughFees\": true,\n          \"shareAmountRounding\": \"CEIL\",\n          \"minimumRate\": 1.49\n        }\n      },\n      \"default\": {\n        \"schema\": {\n          \"rate\": 1.49,\n          \"passThroughFees\": true,\n          \"shareAmountRounding\": \"CEIL\",\n          \"minimumRate\": 1.49\n        }\n      }\n    }\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "a9e4e062-375a-4e76-8986-9a22595373c3",
          "name": "Supported Countries",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "87e2ab01-ed34-4e9c-86df-5cd848cb02cc",
              "name": "List Supported Countries",
              "request": {
                "name": "List Supported Countries",
                "description": {
                  "content": "Retrieves a list of allowed countries for which users can be onboard from.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "countries"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) Filters on the returned countries list has inactive or active countries inside it.",
                        "type": "text/plain"
                      },
                      "key": "status",
                      "value": "<string>"
                    }
                  ],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "d95fdf57-d319-4c3f-9740-316a63914599",
                  "name": "Retrieving a list of Supported Countries was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "countries"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "status",
                          "value": "ACTIVE"
                        }
                      ],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"id\": \"ALA\",\n    \"name\": \"Aland Islands\",\n    \"code2\": \"AX\",\n    \"code3\": \"ALA\",\n    \"active\": true,\n    \"expatsAllowed\": false,\n    \"foreignTINNotRequired\": false,\n    \"fpslProhibited\": false,\n    \"supportDomicile\": false,\n    \"taxTreatyCountry\": false\n  },\n  {\n    \"id\": \"ALA\",\n    \"name\": \"Aland Islands\",\n    \"code2\": \"AX\",\n    \"code3\": \"ALA\",\n    \"active\": true,\n    \"expatsAllowed\": false,\n    \"foreignTINNotRequired\": false,\n    \"fpslProhibited\": false,\n    \"supportDomicile\": false,\n    \"taxTreatyCountry\": false\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "197944a9-18e0-46fa-8702-baf4a8d8b81d",
          "name": "Correspondent Reports",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "324aaf18-6be2-4ca8-ad62-7311aa82ed2a",
              "name": "Retrieve Correspondent Reports",
              "request": {
                "name": "Retrieve Correspondent Reports",
                "description": {
                  "content": "Fetch daily reports generated to provide positions, account activity, balances, and more in file format",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "correspondantReport"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The date for which the Correspondent Report is being requested",
                        "type": "text/plain"
                      },
                      "key": "date",
                      "value": "<string>"
                    }
                  ],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "8c20da2d-5630-44a7-872f-c3cddc25faad",
                  "name": "Fetching Correspondent reports was successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "correspondantReport"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "date",
                          "value": "2023-03-21"
                        }
                      ],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"url\": \"https://dzb6emi8pracf.cloudfront.net/5a013513-8af1-4078-be75-36a5250953f7.1488219178676/Stmt_DRVW_001_DWJM000019_Apr2017.pdf?Policy=eyJTdGF0ZW1lbnQiOiBbeyJSZXNvdXJjZSI6Imh0dHBzOi8vZHpiNmVtaThwcmFjZi5jbG91ZGZyb250Lm5ldC81YTAxMzUxMy04YWYxLTQwNzgtYmU3NS0zNmE1MjUwOTUzZjcuMTQ4ODIxOTE3ODY3Ni9TdG10X0RSVldfMDAxX0RXSk0wMDAwMTlfQXByMjAxNy5wZGYiLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE0OTk3MTc1NDV9LCJJcEFkZHJlc3MiOnsiQVdTOlNvdXJjZUlwIjoiMC4wLjAuMC8wIn19fV19&Signature=UWZRPku4IWoqkp4fyQ179auFVrImZUYDXswjjO-zPGW9-XKno3-TG9O2OHxWG-j7NfEHMXtZbCha~lQwpjt~g58YpL1NYk9xhlp7~HR-skC3J3W8GFVWxbR5TQUXPFOdU-KNwYlTnlE1Wr81nUyoNWrrF-8afyiHVnfm2w35GpZavAKhOiKNDHn7kTorQz3rbkYDks9u1CGPU7TCeZ-GzupVqsUN7xDOxPUnH0KCVGY86PT8bEpPkhpc3jNmtLnB~WB3YdrFg0bSbrbU4M-sVyp49AqK~xq5uDu3Bx22vdyJlKUClEsVvKhQLOArkpMdHYwyPZC~Kz85sroGqnP3oQ__&Key-Pair-Id=APKAJP3MFGZ6DRA4CW4Q\"\n}",
                  "cookie": []
                },
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "769393b0-45a8-49c3-93c6-bc5291604855",
                  "name": "Bad Request",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "correspondantReport"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "date",
                          "value": "2023-03-21"
                        }
                      ],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "Bad Request",
                  "code": 400,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"errorCode\": \"E031\",\n  \"message\": \"Invalid or missing parameters in the request URL or body. Refer to the API documentation for details. Details: Required : [date]\"\n}",
                  "cookie": []
                },
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "2a1e8458-b62f-49f3-b54b-9608775a40ff",
                  "name": "Internal Server Error",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "correspondantReport"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "date",
                          "value": "2023-03-21"
                        }
                      ],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "Internal Server Error",
                  "code": 500,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"errorCode\": \"laborum\",\n  \"message\": \"quis deserunt magna\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "b5e98d38-060f-461a-ab7f-dc60989f96b1",
          "name": "Risk",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [],
          "event": []
        }
      ],
      "event": []
    },
    {
      "id": "88fb08e4-eacd-4bdd-8337-c3faeb133e7c",
      "name": "Money Movement APIs",
      "item": [
        {
          "id": "ad55733b-c5ec-4348-ba4f-9d3c6468aee3",
          "name": "Linked Bank Accounts",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "b076515b-02ac-4884-9049-e6caab18c5de",
              "name": "List User Linked Bank Accounts",
              "request": {
                "name": "List User Linked Bank Accounts",
                "description": {
                  "content": "Retrieves a list of User Linked Bank Accounts by userID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "users",
                    ":userID",
                    "bank-accounts"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) Unique ID of the User to fetch their stored bank accounts.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "userID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "e3e31e7f-e447-4666-81c0-aeec2144bf83",
                  "name": "Retrieving a list of User Linked Bank Accounts was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "users",
                        ":userID",
                        "bank-accounts"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) Unique ID of the User to fetch their stored bank accounts.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "userID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"id\": \"bank_a4656e60-321e-425b-aa0d-a2e75c38885f\",\n    \"bankAccountDetails\": {\n      \"bankAccountNickName\": \"PREFERRED CHECKING\",\n      \"bankAccountNumber\": \"****3174\",\n      \"bankRoutingNumber\": \"110000000\"\n    },\n    \"default\": \"mollit aliqua \",\n    \"status\": \"ACTIVE\",\n    \"created\": \"2022-12-11T22:28:21.810Z\",\n    \"updated\": \"2022-12-11T22:28:21.810Z\"\n  },\n  {\n    \"id\": \"bank_a4656e60-321e-425b-aa0d-a2e75c38885f\",\n    \"bankAccountDetails\": {\n      \"bankAccountNickName\": \"PREFERRED CHECKING\",\n      \"bankAccountNumber\": \"****3174\",\n      \"bankRoutingNumber\": \"110000000\"\n    },\n    \"default\": \"mollit deseru\",\n    \"status\": \"ACTIVE\",\n    \"created\": \"2022-12-11T22:28:21.810Z\",\n    \"updated\": \"2022-12-11T22:28:21.810Z\"\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "dbf7e596-027f-4dc0-a063-b626fc4e19d5",
          "name": "Virtual Bank Accounts",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "6111a562-5b5a-4e54-8a54-4431ee98685e",
              "name": "Retrieve Account Virtual Bank Account",
              "request": {
                "name": "Retrieve Account Virtual Bank Account",
                "description": {
                  "content": "Retrieves an Account Virtual Bank Account details by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "funding",
                    "deposit-instructions"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "f5e903d8-c26c-4dd7-83c8-a0cbbc9004c8",
                  "name": "Retrieving Virtual Bank Account details by accountID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "funding",
                        "deposit-instructions"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"bank_a4656e60-321e-425b-aa0d-a2e75c38885f\",\n  \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n  \"accountNo\": \"DWBG000052\",\n  \"wireDetails\": {\n    \"bankAccountNumber\": \"7442393174\",\n    \"bankName\": \"JP Morgan Chase\",\n    \"bankSwiftCode\": \"CHASUS33\",\n    \"bankAddress\": {\n      \"addressLine1\": \"222 BROADWAY\",\n      \"city\": \"New York City\",\n      \"stateProvince\": \"New York\",\n      \"zipPostalCode\": \"10038\",\n      \"country\": \"USA\"\n    },\n    \"beneficiaryName\": \"Tom Ace\",\n    \"beneficiaryAddress\": {\n      \"addressLine1\": \"222 BROADWAY\",\n      \"city\": \"New York City\",\n      \"stateProvince\": \"New York\",\n      \"zipPostalCode\": \"10038\",\n      \"country\": \"USA\"\n    },\n    \"virtualAccountID\": \"bfa2e...\",\n    \"paymentType\": \"WIRE\"\n  },\n  \"achDetails\": {\n    \"bankAccountNumber\": \"7442393174\",\n    \"bankRoutingNumber\": \"110000000\",\n    \"bankName\": \"JP Morgan Chase\",\n    \"bankAddress\": {\n      \"addressLine1\": \"222 BROADWAY\",\n      \"city\": \"New York City\",\n      \"stateProvince\": \"New York\",\n      \"zipPostalCode\": \"10038\",\n      \"country\": \"USA\"\n    },\n    \"bankRoutingNumberType\": \"ACH\",\n    \"beneficiaryName\": \"Tom Ace\",\n    \"beneficiaryAddress\": {\n      \"addressLine1\": \"222 BROADWAY\",\n      \"city\": \"New York City\",\n      \"stateProvince\": \"New York\",\n      \"zipPostalCode\": \"10038\",\n      \"country\": \"USA\"\n    },\n    \"virtualAccountID\": \"bfa2e...\",\n    \"paymentType\": \"ACH\"\n  },\n  \"wireDomesticDetails\": {\n    \"bankAccountNumber\": \"7442393174\",\n    \"bankRoutingNumber\": \"110000000\",\n    \"bankName\": \"JP Morgan Chase\",\n    \"bankAddress\": {\n      \"addressLine1\": \"222 BROADWAY\",\n      \"city\": \"New York City\",\n      \"stateProvince\": \"New York\",\n      \"zipPostalCode\": \"10038\",\n      \"country\": \"USA\"\n    },\n    \"bankRoutingNumberType\": \"ABA\",\n    \"beneficiaryName\": \"Tom Ace\",\n    \"beneficiaryAddress\": {\n      \"addressLine1\": \"222 BROADWAY\",\n      \"city\": \"New York City\",\n      \"stateProvince\": \"New York\",\n      \"zipPostalCode\": \"10038\",\n      \"country\": \"USA\"\n    },\n    \"virtualAccountID\": \"bfa2e...\",\n    \"paymentType\": \"WIRE\"\n  }\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "4ad04eef-1bf4-4133-a348-a0b90bb2acb3",
          "name": "Deposits",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "f5fbcc2a-3684-4811-adc1-6240a7a8c751",
              "name": "List Account Deposits",
              "request": {
                "name": "List Account Deposits",
                "description": {
                  "content": "Retrieves a list of Account Deposits by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "funding",
                    "deposits"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "a52109a7-70e7-494c-b2f4-78b60dcdebe4",
                  "name": "Retrieving a list of Account Deposits was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "funding",
                        "deposits"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"CKDQ000001-1671085040913-DMIQY\",\n  \"paymentID\": \"CKDQ000001-1671085040913-DMIQY\",\n  \"amount\": 125.22,\n  \"currency\": {\n    \"name\": \"USD\",\n    \"description\": \"US Dollar\",\n    \"symbol\": \"$\"\n  },\n  \"status\": {\n    \"id\": 1,\n    \"message\": \"PENDING\",\n    \"updated\": \"2022-12-11T22:28:21.810Z\"\n  },\n  \"accountDetails\": {\n    \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n    \"accountNo\": \"DWBG000052\",\n    \"accountType\": {\n      \"name\": \"LIVE\",\n      \"description\": \"Live Account\"\n    },\n    \"accountManagementType\": {\n      \"name\": \"SELF\",\n      \"description\": \"Self Directed Account\"\n    }\n  },\n  \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n  \"note\": \"Hey! Welcome to DriveWealth Developer Docs!\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "f2b1f28a-e0a8-4616-9e03-8405278c899f",
              "name": "Create Deposit",
              "request": {
                "name": "Create Deposit",
                "description": {
                  "content": "Creates a Deposit.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "funding",
                    "deposits"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": []
                },
                "header": [
                  {
                    "disabled": false,
                    "description": {
                      "content": "A unique key (UUID) that is used to prevent duplicate requests. Should a network interruption occur, or you otherwise lost a response from the API, you can safely perform the request provided that you send the same value as the Idempotency-Key. DriveWealth Idempotency Keys are saved for 4 days. Within this time period, sending any request with a duplicate key will return the exact same response as the original request, including the same status code and payload.",
                      "type": "text/plain"
                    },
                    "key": "Idempotency-Key",
                    "value": "<string>"
                  },
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "POST",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"accountNo\": \"<string>\",\n  \"amount\": \"<number>\",\n  \"currency\": \"<string>\",\n  \"type\": \"<string>\",\n  \"bankAccountID\": \"<string>\",\n  \"note\": \"<string>\",\n  \"iraContribution\": \"<string>\",\n  \"recurringFrequency\": \"<string>\",\n  \"startDate\": \"<string>\",\n  \"settlementProfileID\": \"<string>\",\n  \"originatorBankDetails\": {\n    \"bankAccountNumber\": \"<string>\",\n    \"bankRoutingNumber\": \"<string>\",\n    \"bankName\": \"<string>\",\n    \"bankAddress\": \"<string>\",\n    \"bankAccountCountry\": \"<string>\",\n    \"accountHolderName\": \"<string>\",\n    \"accountHolderAddress\": \"<string>\",\n    \"accountHolderCountry\": \"<string>\"\n  },\n  \"metadata\": \"<object>\"\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "393839fd-94df-49f4-953b-5c25045ddf2c",
                  "name": "Creating a User's Account Deposit was successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "funding",
                        "deposits"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": []
                    },
                    "header": [
                      {
                        "disabled": false,
                        "description": {
                          "content": "A unique key (UUID) that is used to prevent duplicate requests. Should a network interruption occur, or you otherwise lost a response from the API, you can safely perform the request provided that you send the same value as the Idempotency-Key. DriveWealth Idempotency Keys are saved for 4 days. Within this time period, sending any request with a duplicate key will return the exact same response as the original request, including the same status code and payload.",
                          "type": "text/plain"
                        },
                        "key": "Idempotency-Key",
                        "value": "a1b2c3d4-5e6f-7g8h-9i0j-1k2l3m4n5o6"
                      },
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"accountNo\": \"DWFS001102\",\n  \"amount\": 100.25,\n  \"currency\": \"USD\",\n  \"type\": \"ACH\",\n  \"bankAccountID\": \"bank_a4656e60-321e-425b-aa0d-a2e75c38885f\"\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"CKDQ000001-1671085040913-DMIQY\",\n  \"accountNo\": \"DWBG000052\",\n  \"category\": \"DEPOSIT\",\n  \"currency\": \"USD\",\n  \"amount\": 250.25,\n  \"status\": \"PENDING\",\n  \"source\": {\n    \"id\": \"ACH\",\n    \"brand\": \"ACH\",\n    \"meta_info\": \"Hey! Welcome to DriveWealth Developer Docs!\"\n  },\n  \"created\": \"2022-12-11T22:28:21.810Z\",\n  \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n  \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n  \"transactionCode\": \"JOURNAL\",\n  \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n  \"batch\": true,\n  \"recurring\": {\n    \"id\": \"recurring_98be6652-6361-4d4c-905b-06e9ec38d060\",\n    \"nextDeposit\": \"2019-01-15\",\n    \"active\": false,\n    \"frequency\": \"MONTHLY_FIRST\"\n  }\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "abc7aba2-76d7-4e6c-8fe6-39a52c7d1f4d",
              "name": "Retrieve Deposit",
              "request": {
                "name": "Retrieve Deposit",
                "description": {
                  "content": "Retrieves Deposit details by depositID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "funding",
                    "deposits",
                    ":depositID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) A unique identifier for the user's account deposit.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "depositID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "0e99d699-b912-4879-9377-66058536289a",
                  "name": "Retrieving a Deposit by depositID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "funding",
                        "deposits",
                        ":depositID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) A unique identifier for the user's account deposit.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "depositID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n  \"category\": \"DEPOSIT\",\n  \"amount\": 250.25,\n  \"currency\": {\n    \"name\": \"USD\",\n    \"description\": \"US Dollar\",\n    \"symbol\": \"$\"\n  },\n  \"status\": \"PENDING\",\n  \"created\": \"2022-12-11T22:28:21.810Z\",\n  \"userDetails\": {\n    \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n    \"username\": \"ttc.user.justin\",\n    \"firstName\": \"Justin\",\n    \"lastName\": \"Smith\",\n    \"email\": \"jj@drivewealth.dev\",\n    \"parentIBID\": {\n      \"id\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9\",\n      \"name\": \"Tendies Trading Company\"\n    },\n    \"wlpID\": \"TTC\"\n  },\n  \"accountDetails\": [\n    {\n      \"id\": \"8b8ba3fd-74dc-45dc-b2dc-7de683bd713c.1556222995391\",\n      \"accountNo\": \"DWBG000052\",\n      \"nickname\": \"Justin's Self Directed Account\",\n      \"status\": {\n        \"name\": \"PENDING\",\n        \"description\": \"Pending\"\n      },\n      \"accountType\": \"LIVE\",\n      \"accountManagementType\": \"SELF\",\n      \"tradingType\": {\n        \"name\": \"CASH\",\n        \"description\": \"Cash Account\"\n      },\n      \"leverage\": 1,\n      \"commissionID\": \"449d41b9-3940-41ff-b0e6-334adfb443f8\",\n      \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n      \"restricted\": false,\n      \"goodFaithViolations\": 0,\n      \"patternDayTrades\": 0,\n      \"freeTradeBalance\": 0,\n      \"gfvPdtExempt\": false,\n      \"buyingPowerOverride\": false,\n      \"bod\": {\n        \"moneyMarket\": 3028.98,\n        \"equityValue\": 12071.5,\n        \"cashAvailableForWithdrawal\": 3028.98,\n        \"cashAvailableForTrading\": 3028.98,\n        \"updatedWhen\": \"2022-12-12T21:13:12.391Z\"\n      },\n      \"cashBalance\": 3028.98,\n      \"sweepInd\": true,\n      \"interestFree\": false,\n      \"createdWhen\": \"2022-12-11T22:28:21.810Z\",\n      \"updatedWhen\": \"2022-12-11T22:28:21.810Z\",\n      \"lastActivityDate\": \"2024-07-23\",\n      \"interestedParties\": [\n        {\n          \"type\": \"AUTHORIZED_USERS\",\n          \"data\": [\n            {\n              \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n            },\n            {\n              \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n            }\n          ]\n        },\n        {\n          \"type\": \"AUTHORIZED_USERS\",\n          \"data\": [\n            {\n              \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n            },\n            {\n              \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n            }\n          ]\n        }\n      ]\n    },\n    {\n      \"id\": \"8b8ba3fd-74dc-45dc-b2dc-7de683bd713c.1556222995391\",\n      \"accountNo\": \"DWBG000052\",\n      \"nickname\": \"Justin's Self Directed Account\",\n      \"status\": {\n        \"name\": \"PENDING\",\n        \"description\": \"Pending\"\n      },\n      \"accountType\": \"LIVE\",\n      \"accountManagementType\": \"SELF\",\n      \"tradingType\": {\n        \"name\": \"CASH\",\n        \"description\": \"Cash Account\"\n      },\n      \"leverage\": 1,\n      \"commissionID\": \"449d41b9-3940-41ff-b0e6-334adfb443f8\",\n      \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n      \"restricted\": false,\n      \"goodFaithViolations\": 0,\n      \"patternDayTrades\": 0,\n      \"freeTradeBalance\": 0,\n      \"gfvPdtExempt\": false,\n      \"buyingPowerOverride\": false,\n      \"bod\": {\n        \"moneyMarket\": 3028.98,\n        \"equityValue\": 12071.5,\n        \"cashAvailableForWithdrawal\": 3028.98,\n        \"cashAvailableForTrading\": 3028.98,\n        \"updatedWhen\": \"2022-12-12T21:13:12.391Z\"\n      },\n      \"cashBalance\": 3028.98,\n      \"sweepInd\": true,\n      \"interestFree\": false,\n      \"createdWhen\": \"2022-12-11T22:28:21.810Z\",\n      \"updatedWhen\": \"2022-12-11T22:28:21.810Z\",\n      \"lastActivityDate\": \"2024-07-23\",\n      \"interestedParties\": [\n        {\n          \"type\": \"AUTHORIZED_USERS\",\n          \"data\": [\n            {\n              \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n            },\n            {\n              \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n            }\n          ]\n        },\n        {\n          \"type\": \"AUTHORIZED_USERS\",\n          \"data\": [\n            {\n              \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n            },\n            {\n              \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n            }\n          ]\n        }\n      ]\n    }\n  ],\n  \"batch\": true,\n  \"transactionCode\": {\n    \"code\": \"JOURNAL\",\n    \"type\": \"CSR\",\n    \"description\": \"Cash Receipt - ACH\"\n  },\n  \"note\": \"Hey! Welcome to DriveWealth Developer Docs!\",\n  \"details\": {\n    \"country\": \"USA\",\n    \"bankAccountNumber\": \"****3174\",\n    \"bankRoutingNumber\": \"****0000\",\n    \"accountHolderName\": \"Justin Smith\"\n  },\n  \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n  \"statusHistory\": [\n    {\n      \"status\": 1,\n      \"statusMessage\": \"PENDING\",\n      \"updatedBy\": \"SYSTEM REPORT SERVICE\",\n      \"comment\": \"Valid request. Auto-move to Pending\"\n    },\n    {\n      \"status\": 1,\n      \"statusMessage\": \"PENDING\",\n      \"updatedBy\": \"INSTANT FUNDING BREAKDOWN JOB\",\n      \"comment\": \"Valid request. Auto-move to Pending\"\n    }\n  ]\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "3305992f-71fc-4024-8a97-6721150975a0",
              "name": "Retrieve Recurring Deposits",
              "request": {
                "name": "Retrieve Recurring Deposits",
                "description": {
                  "content": "Retrieves Recurring Deposits details by recurringID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "funding",
                    "recurring-deposits",
                    ":recurringID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) A unique identifier for the user's recurring bank deposit.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "recurringID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "2154ddfe-f365-4123-92c7-0534789967ba",
                  "name": "Fetching recurring deposit schedule was successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "funding",
                        "recurring-deposits",
                        ":recurringID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) A unique identifier for the user's recurring bank deposit.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "recurringID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"recurring_98be6652-6361-4d4c-905b-06e9ec38d060\",\n  \"currency\": \"USD\",\n  \"amount\": 1075.25,\n  \"frequency\": \"MONTHLY_FIRST\",\n  \"bankAccountID\": \"bank_a4656e60-321e-425b-aa0d-a2e75c38885f\",\n  \"active\": true,\n  \"nextDeposit\": \"2019-01-15\",\n  \"depositHistory\": [\n    {\n      \"depositID\": \"CKDQ000001-1671085040913-DMIQY\",\n      \"currency\": \"USD\",\n      \"status\": \"PENDING\",\n      \"created\": \"2022-12-11T22:28:21.810Z\",\n      \"updated\": \"2022-12-11T22:28:21.810Z\",\n      \"createdBy\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd\",\n      \"metaAccountInfo\": \"Automated DAILY recurring deposit for b25f0d3... |MyBank Premier Checking|****5204\"\n    },\n    {\n      \"depositID\": \"CKDQ000001-1671085040913-DMIQY\",\n      \"currency\": \"USD\",\n      \"status\": \"PENDING\",\n      \"created\": \"2022-12-11T22:28:21.810Z\",\n      \"updated\": \"2022-12-11T22:28:21.810Z\",\n      \"createdBy\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd\",\n      \"metaAccountInfo\": \"Automated DAILY recurring deposit for b25f0d3... |MyBank Premier Checking|****5204\"\n    }\n  ]\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "caa3ac71-308e-4773-b2ef-92720e939843",
              "name": "Update Recurring Deposit",
              "request": {
                "name": "Update Recurring Deposit",
                "description": {
                  "content": "Updates Recurring Deposit details by recurringID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "funding",
                    "recurring-deposits",
                    ":recurringID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) A unique identifier for the user's recurring bank deposit.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "recurringID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "PATCH",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"amount\": \"<number>\",\n  \"frequency\": \"<string>\"\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "20f10974-b556-4ca3-92de-61b5bf957c09",
                  "name": "Updating a User's recurring deposit was successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "funding",
                        "recurring-deposits",
                        ":recurringID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) A unique identifier for the user's recurring bank deposit.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "recurringID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "PATCH",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"amount\": 330.25,\n  \"frequency\": \"MONTHLY_FIRST\"\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"amount\": 330.25,\n  \"frequency\": \"MONTHLY_FIRST\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "0027038a-6511-4134-a563-43c78674d50b",
              "name": "Delete Recurring Deposit",
              "request": {
                "name": "Delete Recurring Deposit",
                "description": {
                  "content": "Deactivates Recurring Deposit details by recurringID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "funding",
                    "recurring-deposits",
                    ":recurringID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) A unique identifier for the user's recurring bank deposit.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "recurringID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "DELETE"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "1f260fe8-6b5c-4da3-a870-e79540d43117",
                  "name": "Deactivating Recurring Deposit was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "funding",
                        "recurring-deposits",
                        ":recurringID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) A unique identifier for the user's recurring bank deposit.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "recurringID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "DELETE",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"recurring_98be6652-6361-4d4c-905b-06e9ec38d060\",\n  \"currency\": \"USD\",\n  \"amount\": 1075.25,\n  \"frequency\": \"MONTHLY_FIRST\",\n  \"bankAccountID\": \"bank_a4656e60-321e-425b-aa0d-a2e75c38885f\",\n  \"active\": false,\n  \"nextDeposit\": \"dolor laboris\",\n  \"depositHistory\": [\n    {\n      \"depositID\": \"CKDQ000001-1671085040913-DMIQY\",\n      \"currency\": \"USD\",\n      \"status\": \"PENDING\",\n      \"created\": \"2022-12-11T22:28:21.810Z\",\n      \"updated\": \"2022-12-11T22:28:21.810Z\",\n      \"createdBy\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd\",\n      \"metaAccountInfo\": \"Automated DAILY recurring deposit for b25f0d3... |MyBank Premier Checking|****5204\"\n    },\n    {\n      \"depositID\": \"CKDQ000001-1671085040913-DMIQY\",\n      \"currency\": \"USD\",\n      \"status\": \"PENDING\",\n      \"created\": \"2022-12-11T22:28:21.810Z\",\n      \"updated\": \"2022-12-11T22:28:21.810Z\",\n      \"createdBy\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd\",\n      \"metaAccountInfo\": \"Automated DAILY recurring deposit for b25f0d3... |MyBank Premier Checking|****5204\"\n    }\n  ],\n  \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n  \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n  \"created\": \"2022-12-11T22:28:21.810Z\",\n  \"updated\": \"2022-12-11T22:28:21.810Z\",\n  \"createdBy\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "530ac982-e7fe-4a88-b95e-9a8081ba4dd4",
              "name": "List User Recurring Deposits",
              "request": {
                "name": "List User Recurring Deposits",
                "description": {
                  "content": "Retrieves a list of User Recurring Deposits by userID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "users",
                    ":userID",
                    "recurring-deposits"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The User's unique identifier.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "userID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "4af63216-5591-425d-82e6-b7d37622fb29",
                  "name": "Fetching All User's Recurring Deposits was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "users",
                        ":userID",
                        "recurring-deposits"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) The User's unique identifier.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "userID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"id\": \"recurring_98be6652-6361-4d4c-905b-06e9ec38d060\",\n    \"currency\": \"USD\",\n    \"amount\": 1075.25,\n    \"frequency\": \"MONTHLY_FIRST\",\n    \"bankAccountID\": \"bank_a4656e60-321e-425b-aa0d-a2e75c38885f\",\n    \"active\": true,\n    \"nextDeposit\": \"2019-01-15\",\n    \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n    \"created\": \"2022-12-11T22:28:21.810Z\",\n    \"updated\": \"2022-12-11T22:28:21.810Z\",\n    \"createdBy\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd\"\n  },\n  {\n    \"id\": \"recurring_98be6652-6361-4d4c-905b-06e9ec38d060\",\n    \"currency\": \"USD\",\n    \"amount\": 1075.25,\n    \"frequency\": \"MONTHLY_FIRST\",\n    \"bankAccountID\": \"bank_a4656e60-321e-425b-aa0d-a2e75c38885f\",\n    \"active\": true,\n    \"nextDeposit\": \"2019-01-15\",\n    \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n    \"created\": \"2022-12-11T22:28:21.810Z\",\n    \"updated\": \"2022-12-11T22:28:21.810Z\",\n    \"createdBy\": \"b25f0d36-b4e4-41f8-b3d9-9249e46402cd\"\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "49ff0b0d-bf98-4a9c-96f9-508c8e22c359",
              "name": "List User Deposits",
              "request": {
                "name": "List User Deposits",
                "description": {
                  "content": "Retrieves a list of User Deposits by userID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "users",
                    ":userID",
                    "funding",
                    "deposits"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The User's unique identifier.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "userID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "081d1b32-ebe8-40c3-80a1-92a19eb663fa",
                  "name": "Retrieving a list User Deposits by userID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "users",
                        ":userID",
                        "funding",
                        "deposits"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) The User's unique identifier.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "userID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"id\": \"CKDQ000001-1671085040913-DMIQY\",\n    \"paymentID\": \"CKDQ000001-1671085040913-DMIQY\",\n    \"amount\": 125.22,\n    \"currency\": {\n      \"name\": \"USD\",\n      \"description\": \"US Dollar\",\n      \"symbol\": \"$\"\n    },\n    \"status\": {\n      \"id\": 1,\n      \"message\": \"PENDING\",\n      \"updated\": \"2022-12-11T22:28:21.810Z\"\n    },\n    \"accountDetails\": {\n      \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n      \"accountNo\": \"DWBG000052\",\n      \"accountType\": {\n        \"name\": \"LIVE\",\n        \"description\": \"Live Account\"\n      },\n      \"accountManagementType\": {\n        \"name\": \"SELF\",\n        \"description\": \"Self Directed Account\"\n      }\n    },\n    \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n    \"note\": \"Hey! Welcome to DriveWealth Developer Docs!\"\n  },\n  {\n    \"id\": \"CKDQ000001-1671085040913-DMIQY\",\n    \"paymentID\": \"CKDQ000001-1671085040913-DMIQY\",\n    \"amount\": 125.22,\n    \"currency\": {\n      \"name\": \"USD\",\n      \"description\": \"US Dollar\",\n      \"symbol\": \"$\"\n    },\n    \"status\": {\n      \"id\": 1,\n      \"message\": \"PENDING\",\n      \"updated\": \"2022-12-11T22:28:21.810Z\"\n    },\n    \"accountDetails\": {\n      \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n      \"accountNo\": \"DWBG000052\",\n      \"accountType\": {\n        \"name\": \"LIVE\",\n        \"description\": \"Live Account\"\n      },\n      \"accountManagementType\": {\n        \"name\": \"SELF\",\n        \"description\": \"Self Directed Account\"\n      }\n    },\n    \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n    \"note\": \"Hey! Welcome to DriveWealth Developer Docs!\"\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "7998b704-b404-4a11-9756-10ef88cfa8d1",
          "name": "Withdrawals",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "9c16f5ff-ffeb-4d9a-a0aa-f81c38f5a683",
              "name": "List Account Withdrawals",
              "request": {
                "name": "List Account Withdrawals",
                "description": {
                  "content": "Retrieves a list of Account Withdrawals by accountID",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "funding",
                    "redemptions"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "99ecddf7-dbd0-465e-84c3-795245610d7e",
                  "name": "Retrieving a list of Account Withdrawals was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "funding",
                        "redemptions"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"id\": \"DWUV000006-1593451797743-R8CC7\",\n    \"paymentID\": \"DWUV000006-1593451797743-R8CC7\",\n    \"amount\": 250.25,\n    \"currency\": {\n      \"name\": \"USD\",\n      \"description\": \"US Dollar\",\n      \"symbol\": \"$\"\n    },\n    \"status\": {\n      \"id\": 1,\n      \"message\": \"PENDING\",\n      \"updated\": \"2022-12-11T22:28:21.810Z\"\n    },\n    \"accountDetails\": {\n      \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n      \"accountNo\": \"DWBG000052\",\n      \"accountType\": {\n        \"name\": \"LIVE\",\n        \"description\": \"Live Account\"\n      },\n      \"accountManagementType\": {\n        \"name\": \"SELF\",\n        \"description\": \"Self Directed Account\"\n      }\n    },\n    \"fees\": [\n      {\n        \"type\": \"FEE_ACH\",\n        \"amount\": -5.99,\n        \"description\": \"Fee - ACH\",\n        \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n        \"transactionCode\": \"JOURNAL\",\n        \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n        \"created\": \"2022-12-11T22:28:21.810Z\",\n        \"currency\": \"USD\",\n        \"symbol\": \"$\"\n      },\n      {\n        \"type\": \"FEE_ACH\",\n        \"amount\": -5.99,\n        \"description\": \"Fee - ACH\",\n        \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n        \"transactionCode\": \"JOURNAL\",\n        \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n        \"created\": \"2022-12-11T22:28:21.810Z\",\n        \"currency\": \"USD\",\n        \"symbol\": \"$\"\n      }\n    ],\n    \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n    \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n    \"timestamp\": \"2022-12-11T22:28:21.810Z\"\n  },\n  {\n    \"id\": \"DWUV000006-1593451797743-R8CC7\",\n    \"paymentID\": \"DWUV000006-1593451797743-R8CC7\",\n    \"amount\": 250.25,\n    \"currency\": {\n      \"name\": \"USD\",\n      \"description\": \"US Dollar\",\n      \"symbol\": \"$\"\n    },\n    \"status\": {\n      \"id\": 1,\n      \"message\": \"PENDING\",\n      \"updated\": \"2022-12-11T22:28:21.810Z\"\n    },\n    \"accountDetails\": {\n      \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n      \"accountNo\": \"DWBG000052\",\n      \"accountType\": {\n        \"name\": \"LIVE\",\n        \"description\": \"Live Account\"\n      },\n      \"accountManagementType\": {\n        \"name\": \"SELF\",\n        \"description\": \"Self Directed Account\"\n      }\n    },\n    \"fees\": [\n      {\n        \"type\": \"FEE_ACH\",\n        \"amount\": -5.99,\n        \"description\": \"Fee - ACH\",\n        \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n        \"transactionCode\": \"JOURNAL\",\n        \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n        \"created\": \"2022-12-11T22:28:21.810Z\",\n        \"currency\": \"USD\",\n        \"symbol\": \"$\"\n      },\n      {\n        \"type\": \"FEE_ACH\",\n        \"amount\": -5.99,\n        \"description\": \"Fee - ACH\",\n        \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n        \"transactionCode\": \"JOURNAL\",\n        \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n        \"created\": \"2022-12-11T22:28:21.810Z\",\n        \"currency\": \"USD\",\n        \"symbol\": \"$\"\n      }\n    ],\n    \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n    \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n    \"timestamp\": \"2022-12-11T22:28:21.810Z\"\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "7a553d28-14d9-43a3-ac15-3d3a77dbcfd4",
              "name": "Create Withdrawal",
              "request": {
                "name": "Create Withdrawal",
                "description": {
                  "content": "Creates a Withdrawal.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "funding",
                    "redemptions"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": []
                },
                "header": [
                  {
                    "disabled": false,
                    "description": {
                      "content": "A unique key (UUID) that is used to prevent duplicate requests. Should a network interruption occur, or you otherwise lost a response from the API, you can safely perform the request provided that you send the same value as the Idempotency-Key. DriveWealth Idempotency Keys are saved for 4 days. Within this time period, sending any request with a duplicate key will return the exact same response as the original request, including the same status code and payload.",
                      "type": "text/plain"
                    },
                    "key": "Idempotency-Key",
                    "value": "<string>"
                  },
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "POST",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"accountNo\": \"<string>\",\n  \"amount\": \"<number>\",\n  \"currency\": \"<string>\",\n  \"type\": \"<string>\",\n  \"details\": {\n    \"beneficiaryName\": \"<string>\",\n    \"beneficiaryAccountNumber\": \"<string>\",\n    \"beneficiaryAccountType\": \"<string>\",\n    \"beneficiaryRoutingNumber\": \"<string>\",\n    \"beneficiarySwiftABA\": \"<string>\",\n    \"beneficiaryBankName\": \"<string>\",\n    \"beneficiaryBankAddress\": \"<string>\",\n    \"beneficiaryBankCity\": \"<string>\",\n    \"beneficiaryBankProvince\": \"<string>\",\n    \"beneficiaryBankZip\": \"<string>\",\n    \"beneficiaryBankCountry\": \"<string>\",\n    \"intermediarySwift\": \"<string>\",\n    \"intermediaryBankName\": \"<string>\"\n  },\n  \"bankAccountID\": \"<string>\",\n  \"iraTaxWithholdings\": {\n    \"federalTaxPercentage\": \"<number>\"\n  },\n  \"liquidate\": \"<boolean>\",\n  \"fees\": [\n    {\n      \"type\": \"<string>\",\n      \"amount\": \"<number>\",\n      \"description\": \"<string>\",\n      \"wlpFinTranTypeID\": \"<string>\",\n      \"transactionCode\": \"<string>\",\n      \"finTranReference\": \"<string>\",\n      \"created\": \"<string>\",\n      \"currency\": \"<string>\",\n      \"symbol\": \"<string>\"\n    },\n    {\n      \"type\": \"<string>\",\n      \"amount\": \"<number>\",\n      \"description\": \"<string>\",\n      \"wlpFinTranTypeID\": \"<string>\",\n      \"transactionCode\": \"<string>\",\n      \"finTranReference\": \"<string>\",\n      \"created\": \"<string>\",\n      \"currency\": \"<string>\",\n      \"symbol\": \"<string>\"\n    }\n  ],\n  \"note\": \"<string>\",\n  \"settlementProfileID\": \"<string>\"\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "d0a99cfe-bcb6-43d8-a8dc-369e8bab7d0f",
                  "name": "Creating a User's Account Withdrawal was successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "funding",
                        "redemptions"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": []
                    },
                    "header": [
                      {
                        "disabled": false,
                        "description": {
                          "content": "A unique key (UUID) that is used to prevent duplicate requests. Should a network interruption occur, or you otherwise lost a response from the API, you can safely perform the request provided that you send the same value as the Idempotency-Key. DriveWealth Idempotency Keys are saved for 4 days. Within this time period, sending any request with a duplicate key will return the exact same response as the original request, including the same status code and payload.",
                          "type": "text/plain"
                        },
                        "key": "Idempotency-Key",
                        "value": "a1b2c3d4-5e6f-7g8h-9i0j-1k2l3m4n5o6"
                      },
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"accountNo\": \"DWBG000052\",\n  \"amount\": 125.92,\n  \"currency\": \"USD\",\n  \"type\": \"ACH\",\n  \"details\": {\n    \"beneficiaryName\": \"Justin Smith\",\n    \"beneficiaryAccountNumber\": \"00257596002028990212396\",\n    \"beneficiaryAccountType\": \"CHECKING\",\n    \"beneficiaryRoutingNumber\": \"021000322\",\n    \"beneficiarySwiftABA\": \"BOFAUS3NXXX\",\n    \"beneficiaryBankName\": \"Bank of America\",\n    \"beneficiaryBankAddress\": \"222 BROADWAY\",\n    \"beneficiaryBankCity\": \"New York City\",\n    \"beneficiaryBankProvince\": \"New York\",\n    \"beneficiaryBankZip\": \"10038\",\n    \"beneficiaryBankCountry\": \"USA\",\n    \"intermediarySwift\": \"CHASUS3AXXX\",\n    \"intermediaryBankName\": \"J.P Morgan Chase & Co.\"\n  },\n  \"bankAccountID\": \"bank_a4656e60-321e-425b-aa0d-a2e75c38885f\",\n  \"iraTaxWithholdings\": {\n    \"federalTaxPercentage\": 0.1\n  },\n  \"liquidate\": false,\n  \"fees\": [\n    {\n      \"type\": \"FEE_ACH\",\n      \"amount\": -5.99,\n      \"description\": \"Fee - ACH\",\n      \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n      \"transactionCode\": \"JOURNAL\",\n      \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n      \"created\": \"2022-12-11T22:28:21.810Z\",\n      \"currency\": \"USD\",\n      \"symbol\": \"$\"\n    },\n    {\n      \"type\": \"FEE_ACH\",\n      \"amount\": -5.99,\n      \"description\": \"Fee - ACH\",\n      \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n      \"transactionCode\": \"JOURNAL\",\n      \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n      \"created\": \"2022-12-11T22:28:21.810Z\",\n      \"currency\": \"USD\",\n      \"symbol\": \"$\"\n    }\n  ],\n  \"note\": \"Hey! Welcome to DriveWealth Developer Docs!\",\n  \"settlementProfileID\": \"settlement-profile-bank-account-1\"\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"ZYNN000001-1672169822525-RIUIN\",\n  \"accountNo\": \"DWBG000052\",\n  \"category\": \"REDEMPTION\",\n  \"currency\": \"USD\",\n  \"amount\": -560.36,\n  \"status\": {\n    \"id\": 1,\n    \"message\": \"PENDING\",\n    \"updated\": \"2022-12-11T22:28:21.810Z\"\n  },\n  \"source\": {\n    \"id\": \"ACH\",\n    \"meta_info\": \"Hey! Welcome to DriveWealth Developer Docs!\"\n  },\n  \"paymentRef\": \"ZYNN000001-1672169822525-RIUIN\",\n  \"created\": \"2022-12-08T18:36:40.609Z\",\n  \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n  \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n  \"transactionCode\": \"JOURNAL\",\n  \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n  \"batch\": true,\n  \"account_number\": \"DWBG000052\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "033f52fd-ef50-436c-bda9-ec2c8a0690f6",
              "name": "List Withdrawals",
              "request": {
                "name": "List Withdrawals",
                "description": {
                  "content": "Retrieves a list of Withdrawals.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "funding",
                    "redemptions"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The current status of the withdrawal; to filter by.",
                        "type": "text/plain"
                      },
                      "key": "status",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The type of withdrawal; to filter by.",
                        "type": "text/plain"
                      },
                      "key": "type",
                      "value": "<string>"
                    }
                  ],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "f89d2904-4181-49dd-864a-3440626df8eb",
                  "name": "Retrieving a list of Withdrawals was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "funding",
                        "redemptions"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "status",
                          "value": "PENDING"
                        },
                        {
                          "key": "type",
                          "value": "ACH"
                        }
                      ],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"id\": \"ZYNN000001-1672169822525-RIUIN\",\n    \"paymentID\": \"ZYNN000001-1672169822525-RIUIN\",\n    \"type\": \"ACH\",\n    \"amount\": 125.92,\n    \"currency\": {\n      \"name\": \"USD\",\n      \"description\": \"US Dollar\",\n      \"symbol\": \"$\"\n    },\n    \"status\": {\n      \"id\": 1,\n      \"message\": \"PENDING\",\n      \"updated\": \"2022-12-11T22:28:21.810Z\"\n    },\n    \"userDetails\": {\n      \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n      \"username\": \"ttc.user.justin\",\n      \"firstName\": \"Justin\",\n      \"lastName\": \"Smith\",\n      \"email\": \"jj@drivewealth.dev\",\n      \"parentIBID\": {\n        \"id\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9\",\n        \"name\": \"Tendies Trading Company\"\n      },\n      \"wlpID\": \"TTC\"\n    },\n    \"accountDetails\": {\n      \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n      \"accountNo\": \"DWBG000052\",\n      \"accountType\": {\n        \"name\": \"LIVE\",\n        \"description\": \"Live Account\"\n      },\n      \"accountManagementType\": {\n        \"name\": \"SELF\",\n        \"description\": \"Self Directed Account\"\n      }\n    },\n    \"fees\": [\n      {\n        \"type\": \"FEE_ACH\",\n        \"amount\": -5.99,\n        \"description\": \"Fee - ACH\",\n        \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n        \"transactionCode\": \"JOURNAL\",\n        \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n        \"created\": \"2022-12-11T22:28:21.810Z\",\n        \"currency\": \"USD\",\n        \"symbol\": \"$\"\n      },\n      {\n        \"type\": \"FEE_ACH\",\n        \"amount\": -5.99,\n        \"description\": \"Fee - ACH\",\n        \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n        \"transactionCode\": \"JOURNAL\",\n        \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n        \"created\": \"2022-12-11T22:28:21.810Z\",\n        \"currency\": \"USD\",\n        \"symbol\": \"$\"\n      }\n    ],\n    \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n    \"transactionCode\": {\n      \"code\": \"JOURNAL\",\n      \"type\": \"CSR\",\n      \"description\": \"Cash Receipt - ACH\"\n    }\n  },\n  {\n    \"id\": \"ZYNN000001-1672169822525-RIUIN\",\n    \"paymentID\": \"ZYNN000001-1672169822525-RIUIN\",\n    \"type\": \"ACH\",\n    \"amount\": 125.92,\n    \"currency\": {\n      \"name\": \"USD\",\n      \"description\": \"US Dollar\",\n      \"symbol\": \"$\"\n    },\n    \"status\": {\n      \"id\": 1,\n      \"message\": \"PENDING\",\n      \"updated\": \"2022-12-11T22:28:21.810Z\"\n    },\n    \"userDetails\": {\n      \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n      \"username\": \"ttc.user.justin\",\n      \"firstName\": \"Justin\",\n      \"lastName\": \"Smith\",\n      \"email\": \"jj@drivewealth.dev\",\n      \"parentIBID\": {\n        \"id\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9\",\n        \"name\": \"Tendies Trading Company\"\n      },\n      \"wlpID\": \"TTC\"\n    },\n    \"accountDetails\": {\n      \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n      \"accountNo\": \"DWBG000052\",\n      \"accountType\": {\n        \"name\": \"LIVE\",\n        \"description\": \"Live Account\"\n      },\n      \"accountManagementType\": {\n        \"name\": \"SELF\",\n        \"description\": \"Self Directed Account\"\n      }\n    },\n    \"fees\": [\n      {\n        \"type\": \"FEE_ACH\",\n        \"amount\": -5.99,\n        \"description\": \"Fee - ACH\",\n        \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n        \"transactionCode\": \"JOURNAL\",\n        \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n        \"created\": \"2022-12-11T22:28:21.810Z\",\n        \"currency\": \"USD\",\n        \"symbol\": \"$\"\n      },\n      {\n        \"type\": \"FEE_ACH\",\n        \"amount\": -5.99,\n        \"description\": \"Fee - ACH\",\n        \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n        \"transactionCode\": \"JOURNAL\",\n        \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n        \"created\": \"2022-12-11T22:28:21.810Z\",\n        \"currency\": \"USD\",\n        \"symbol\": \"$\"\n      }\n    ],\n    \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n    \"transactionCode\": {\n      \"code\": \"JOURNAL\",\n      \"type\": \"CSR\",\n      \"description\": \"Cash Receipt - ACH\"\n    }\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "742af645-4f4e-484b-a5c6-f22e381c515a",
              "name": "Retrieve Withdrawal",
              "request": {
                "name": "Retrieve Withdrawal",
                "description": {
                  "content": "Retrieves a Withdrawal by redemptionID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "funding",
                    "redemptions",
                    ":redemptionID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) A unique identifier for the user's account redemption/withdrawal.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "redemptionID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "773e2c47-d8f1-4ad9-a18e-9a997fe10018",
                  "name": "Retrieving a Withdrawal by redemptionID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "funding",
                        "redemptions",
                        ":redemptionID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) A unique identifier for the user's account redemption/withdrawal.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "redemptionID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"ZYNN000001-1672169822525-RIUIN\",\n  \"category\": \"REDEMPTION\",\n  \"currency\": {\n    \"name\": \"USD\",\n    \"description\": \"US Dollar\",\n    \"symbol\": \"$\"\n  },\n  \"status\": {\n    \"id\": 1,\n    \"message\": \"PENDING\",\n    \"updated\": \"2022-12-11T22:28:21.810Z\"\n  },\n  \"created\": \"2022-12-11T22:28:21.810Z\",\n  \"userDetails\": {\n    \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n    \"username\": \"ttc.user.justin\",\n    \"firstName\": \"Justin\",\n    \"lastName\": \"Smith\",\n    \"email\": \"jj@drivewealth.dev\",\n    \"parentIBID\": {\n      \"id\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9\",\n      \"name\": \"Tendies Trading Company\"\n    },\n    \"wlpID\": \"TTC\"\n  },\n  \"accountDetails\": {\n    \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n    \"accountNo\": \"DWBG000052\",\n    \"accountType\": {\n      \"name\": \"LIVE\",\n      \"description\": \"Live Account\"\n    },\n    \"accountManagementType\": {\n      \"name\": \"SELF\",\n      \"description\": \"Self Directed Account\"\n    }\n  },\n  \"batch\": true,\n  \"transactionCode\": {\n    \"code\": \"JOURNAL\",\n    \"type\": \"CSR\",\n    \"description\": \"Cash Receipt - ACH\"\n  },\n  \"statusHistory\": [\n    {\n      \"status\": 1,\n      \"statusMessage\": \"PENDING\",\n      \"created\": \"2022-12-11T22:28:21.810Z\",\n      \"updatedBy\": \"INSTANT FUNDING BREAKDOWN JOB\",\n      \"comment\": \"New redemption request from the back-office\"\n    },\n    {\n      \"status\": 1,\n      \"statusMessage\": \"PENDING\",\n      \"created\": \"2022-12-11T22:28:21.810Z\",\n      \"updatedBy\": \"SYSTEM REPORT SERVICE\",\n      \"comment\": \"New redemption request from the back-office\"\n    }\n  ],\n  \"details\": {\n    \"beneficiaryName\": \"Justin Smith\",\n    \"beneficiaryAccountNumber\": \"00257596002028990212396\",\n    \"beneficiaryAccountType\": \"CHECKING\",\n    \"beneficiaryRoutingNumber\": \"021000322\",\n    \"beneficiarySwiftABA\": \"BOFAUS3NXXX\",\n    \"beneficiaryBankName\": \"Bank of America\",\n    \"beneficiaryBankAddress\": \"222 BROADWAY\",\n    \"beneficiaryBankCity\": \"New York City\",\n    \"beneficiaryBankProvince\": \"New York\",\n    \"beneficiaryBankZip\": \"10038\",\n    \"beneficiaryBankCountry\": \"USA\",\n    \"intermediarySwift\": \"CHASUS3AXXX\",\n    \"intermediaryBankName\": \"J.P Morgan Chase & Co.\"\n  },\n  \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n  \"fees\": [\n    {\n      \"type\": \"FEE_ACH\",\n      \"amount\": -5.99,\n      \"description\": \"Fee - ACH\",\n      \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n      \"transactionCode\": \"JOURNAL\",\n      \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n      \"created\": \"2022-12-11T22:28:21.810Z\",\n      \"currency\": \"USD\",\n      \"symbol\": \"$\"\n    },\n    {\n      \"type\": \"FEE_ACH\",\n      \"amount\": -5.99,\n      \"description\": \"Fee - ACH\",\n      \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n      \"transactionCode\": \"JOURNAL\",\n      \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n      \"created\": \"2022-12-11T22:28:21.810Z\",\n      \"currency\": \"USD\",\n      \"symbol\": \"$\"\n    }\n  ],\n  \"note\": \"Hey! Welcome to DriveWealth Developer Docs!\",\n  \"type\": \"ACH\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "8a8a57e4-4e81-41c2-b2d8-4dcbd3750bf1",
              "name": "List User Withdrawals",
              "request": {
                "name": "List User Withdrawals",
                "description": {
                  "content": "Retrieves a list of User Withdrawals by userID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "users",
                    ":userID",
                    "funding",
                    "redemptions"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The User's unique identifier.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "userID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "db1cf3b2-94a5-4b4f-8e12-b30f117f561b",
                  "name": "Retrieving a list of User Withdrawals by userID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "users",
                        ":userID",
                        "funding",
                        "redemptions"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) The User's unique identifier.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "userID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"id\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n    \"paymentID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n    \"amount\": 250.25,\n    \"currency\": {\n      \"name\": \"USD\",\n      \"description\": \"US Dollar\",\n      \"symbol\": \"$\"\n    },\n    \"status\": {\n      \"id\": 1,\n      \"message\": \"PENDING\",\n      \"updated\": \"2022-12-11T22:28:21.810Z\"\n    },\n    \"accountDetails\": {\n      \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n      \"accountNo\": \"DWBG000052\",\n      \"accountType\": {\n        \"name\": \"LIVE\",\n        \"description\": \"Live Account\"\n      },\n      \"accountManagementType\": {\n        \"name\": \"SELF\",\n        \"description\": \"Self Directed Account\"\n      }\n    },\n    \"fees\": [\n      {\n        \"type\": \"FEE_ACH\",\n        \"amount\": -5.99,\n        \"description\": \"Fee - ACH\",\n        \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n        \"transactionCode\": \"JOURNAL\",\n        \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n        \"created\": \"2022-12-11T22:28:21.810Z\",\n        \"currency\": \"USD\",\n        \"symbol\": \"$\"\n      },\n      {\n        \"type\": \"FEE_ACH\",\n        \"amount\": -5.99,\n        \"description\": \"Fee - ACH\",\n        \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n        \"transactionCode\": \"JOURNAL\",\n        \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n        \"created\": \"2022-12-11T22:28:21.810Z\",\n        \"currency\": \"USD\",\n        \"symbol\": \"$\"\n      }\n    ],\n    \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n    \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n    \"timestamp\": \"2022-12-11T22:28:21.810Z\"\n  },\n  {\n    \"id\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n    \"paymentID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n    \"amount\": 250.25,\n    \"currency\": {\n      \"name\": \"USD\",\n      \"description\": \"US Dollar\",\n      \"symbol\": \"$\"\n    },\n    \"status\": {\n      \"id\": 1,\n      \"message\": \"PENDING\",\n      \"updated\": \"2022-12-11T22:28:21.810Z\"\n    },\n    \"accountDetails\": {\n      \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n      \"accountNo\": \"DWBG000052\",\n      \"accountType\": {\n        \"name\": \"LIVE\",\n        \"description\": \"Live Account\"\n      },\n      \"accountManagementType\": {\n        \"name\": \"SELF\",\n        \"description\": \"Self Directed Account\"\n      }\n    },\n    \"fees\": [\n      {\n        \"type\": \"FEE_ACH\",\n        \"amount\": -5.99,\n        \"description\": \"Fee - ACH\",\n        \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n        \"transactionCode\": \"JOURNAL\",\n        \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n        \"created\": \"2022-12-11T22:28:21.810Z\",\n        \"currency\": \"USD\",\n        \"symbol\": \"$\"\n      },\n      {\n        \"type\": \"FEE_ACH\",\n        \"amount\": -5.99,\n        \"description\": \"Fee - ACH\",\n        \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n        \"transactionCode\": \"JOURNAL\",\n        \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n        \"created\": \"2022-12-11T22:28:21.810Z\",\n        \"currency\": \"USD\",\n        \"symbol\": \"$\"\n      }\n    ],\n    \"wlpFinTranTypeID\": \"c43bab85-2916-4831-a0db-66215150a6e4\",\n    \"finTranReference\": \"HG.cd22a78a-8a48-441c-89d2-ea400964a34b\",\n    \"timestamp\": \"2022-12-11T22:28:21.810Z\"\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "63402156-0218-4758-a897-f0d81305eaa6",
          "name": "Asset Transfer",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "222a1d0e-b898-4455-aa59-39a437a7fdd0",
              "name": "Create ACATS Transfer",
              "request": {
                "name": "Create ACATS Transfer",
                "description": {
                  "content": "The Automated Customer Account Transfer Service (ACATS) is a system that facilitates the transfer of securities from one trading account to another at a different brokerage firm or bank.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "asset-transfers",
                    "acats"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "POST",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"source\": \"<string>\",\n  \"destination\": \"<string>\",\n  \"clearingNo\": \"<string>\",\n  \"sourceAccountType\": \"<string>\",\n  \"acatType\": \"<string>\",\n  \"comment\": \"<string>\",\n  \"metadata\": \"<object>\",\n  \"cash\": 0,\n  \"positions\": [\n    {\n      \"quantity\": \"<number>\",\n      \"symbol\": \"<string>\",\n      \"instrumentID\": \"<uuid>\"\n    },\n    {\n      \"quantity\": \"<number>\",\n      \"symbol\": \"<string>\",\n      \"instrumentID\": \"<uuid>\"\n    }\n  ]\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "718ae006-daa6-4e1d-9bd1-4a034cb87d53",
                  "name": "Initiating a transfer was successful",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "asset-transfers",
                        "acats"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"source\": \"DWBG000052\",\n  \"destination\": \"LKKZ000004\",\n  \"clearingNo\": \"0001\",\n  \"sourceAccountType\": \"<string>\",\n  \"acatType\": \"<string>\",\n  \"comment\": \"Hey! Welcome to DriveWealth Developer Docs!\",\n  \"metadata\": {\n    \"myCustomKey\": \"myCustomValue\"\n  },\n  \"cash\": 0,\n  \"positions\": [\n    {\n      \"quantity\": \"<number>\",\n      \"symbol\": \"MS\",\n      \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\"\n    },\n    {\n      \"quantity\": \"<number>\",\n      \"symbol\": \"MS\",\n      \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\"\n    }\n  ]\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"acats_41eb5bdd-8ce2-4471-8fc6-9892da089cd1\",\n  \"source\": \"BROKER0001\",\n  \"sourceAccountID\": \"d6a776bc-be5c-47df-94eb-baf914f1847c.1738660911962\",\n  \"destination\": \"DWXR001004\",\n  \"destinationAccountID\": \"c815c129-27cd-46f2-b316-ab6bde9aff62.1737384219426\",\n  \"clearingNo\": \"0001\",\n  \"status\": {\n    \"name\": \"PENDING\",\n    \"description\": \"Asset transfer request is pending\"\n  },\n  \"type\": {\n    \"name\": \"ACAT\",\n    \"description\": \"ACAT transfer\"\n  },\n  \"acatType\": {\n    \"name\": \"FULL\",\n    \"description\": \"Full Acats Transfer\"\n  },\n  \"sourceAccountType\": {\n    \"name\": \"INDIVIDUAL\",\n    \"description\": \"Individual Account\"\n  },\n  \"positions\": [],\n  \"metadata\": {},\n  \"auditDetails\": [\n    {\n      \"timestamp\": \"2023-07-28T23:56:10.507Z\",\n      \"status\": {\n        \"name\": \"STARTED\",\n        \"description\": \"Asset transfer request has been initiated.\"\n      },\n      \"comment\": \"Transfer request has been submitted in queue\"\n    },\n    {\n      \"timestamp\": \"2023-07-28T23:56:10.645Z\",\n      \"status\": {\n        \"name\": \"PENDING\",\n        \"description\": \"Asset transfer request is pending\"\n      },\n      \"comment\": \"<string>\"\n    }\n  ],\n  \"created\": \"2023-07-28T23:56:10.491Z\",\n  \"updated\": \"2023-07-28T23:56:10.667Z\"\n}",
                  "cookie": []
                },
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "caec441b-ee58-4f09-8eb4-b57373710976",
                  "name": "Bad Request",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "asset-transfers",
                        "acats"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"source\": \"DWBG000052\",\n  \"destination\": \"LKKZ000004\",\n  \"clearingNo\": \"0001\",\n  \"sourceAccountType\": \"<string>\",\n  \"acatType\": \"<string>\",\n  \"comment\": \"Hey! Welcome to DriveWealth Developer Docs!\",\n  \"metadata\": {\n    \"myCustomKey\": \"myCustomValue\"\n  },\n  \"cash\": 0,\n  \"positions\": [\n    {\n      \"quantity\": \"<number>\",\n      \"symbol\": \"MS\",\n      \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\"\n    },\n    {\n      \"quantity\": \"<number>\",\n      \"symbol\": \"MS\",\n      \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\"\n    }\n  ]\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "Bad Request",
                  "code": 400,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"errorCode\": \"A012\",\n  \"message\": \"A required accountNo is missing or invalid. Refer to the API documentation for details.\",\n  \"errorDetails\": {\n    \"field\": \"destination\",\n    \"type\": \"STRING\"\n  }\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "117890ab-010f-4e5b-9156-56b98326cd8b",
              "name": "Create Minor Graduation Transfer",
              "request": {
                "name": "Create Minor Graduation Transfer",
                "description": {
                  "content": "If an Account is opened for the purpose of allowing a minor to invest, this API will allow for the transfer of assets from this account to the minor's own named account once they reach the age of majority.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "asset-transfers",
                    "minor-graduation"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "POST",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"source\": \"<string>\",\n  \"destination\": \"<string>\",\n  \"comment\": \"<string>\",\n  \"metadata\": \"<object>\"\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "36d36b87-672c-4996-a7b3-397a7221d8bc",
                  "name": "Initiating a transfer was successful",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "asset-transfers",
                        "minor-graduation"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"source\": \"LKGE000001\",\n  \"destination\": \"LKKZ000004\",\n  \"comment\": \"Migrating Teen account to Individual account.\",\n  \"metadata\": {}\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"grad_28d08c72-3d0f-4c6e-8961-2dc6491c28a8\",\n  \"source\": \"LKGE000001\",\n  \"destination\": \"LKKZ000004\",\n  \"status\": {\n    \"name\": \"STARTED\",\n    \"description\": \"Asset transfer request has been initiated.\"\n  },\n  \"type\": {\n    \"name\": \"TEEN\",\n    \"description\": \"Teen Account Transfer\"\n  },\n  \"created\": \"2023-07-26T14:05:18.518Z\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "7236258d-8f2e-4b1e-8537-ba54f1272096",
              "name": "Retrieve Transfer",
              "request": {
                "name": "Retrieve Transfer",
                "description": {
                  "content": "Get a Transfer's current details.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "asset-transfers",
                    ":assetTransferID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "assetTransferID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "37b754b5-856b-4e4f-b617-14fa68f5ef13",
                  "name": "OK",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "asset-transfers",
                        ":assetTransferID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "assetTransferID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"acats_0a18eea2-c63d-447a-a0f1-1c7d9a08c9da\",\n  \"source\": \"TR6666\",\n  \"sourceAccountID\": \"d6a776bc-be5c-47df-94eb-baf914f1847c.1738660911962\",\n  \"destination\": \"FWCT000005\",\n  \"destinationAccountID\": \"c815c129-27cd-46f2-b316-ab6bde9aff62.1737384219426\",\n  \"clearingNo\": \"1111\",\n  \"status\": {\n    \"name\": \"SUCCESSFUL\",\n    \"description\": \"Asset transfer request has been successfully completed\"\n  },\n  \"type\": {\n    \"name\": \"ACAT\",\n    \"description\": \"ACAT transfer\"\n  },\n  \"acatType\": {\n    \"name\": \"PARTIAL\",\n    \"description\": \"Partial Acats Transfer\"\n  },\n  \"acatTransit\": {\n    \"name\": \"ACAT_IN\",\n    \"description\": \"Incoming Acats Transfer\"\n  },\n  \"sourceAccountType\": {\n    \"name\": \"INDIVIDUAL\",\n    \"description\": \"Individual Account\"\n  },\n  \"partner\": {\n    \"id\": \"25f77a3e-2a4b-48bf-bea2-1b8bcd541621\",\n    \"name\": \"Stark House\"\n  },\n  \"positions\": [\n    {\n      \"symbol\": \"ACHN\",\n      \"instrumentID\": \"27673f0e-2219-40b0-9ecc-91c87266efaf\",\n      \"quantity\": 1\n    },\n    {\n      \"symbol\": \"SBSI\",\n      \"instrumentID\": \"1c6c1625-8146-4dd3-a84b-c6a97cd74bcf\",\n      \"quantity\": 56\n    }\n  ],\n  \"metadata\": {},\n  \"auditDetails\": [\n    {\n      \"timestamp\": \"2023-10-20T13:02:50.970Z\",\n      \"status\": {\n        \"name\": \"STARTED\",\n        \"description\": \"Asset transfer request has been initiated.\"\n      },\n      \"comment\": \"Transfer request has been submitted in queue\"\n    },\n    {\n      \"timestamp\": \"2023-10-20T15:00:04.185Z\",\n      \"status\": {\n        \"name\": \"PENDING\",\n        \"description\": \"Asset transfer request is pending\"\n      },\n      \"comment\": \"TIF has been created\"\n    },\n    {\n      \"timestamp\": \"2023-11-02T00:01:19.340Z\",\n      \"status\": {\n        \"name\": \"SUCCESSFUL\",\n        \"description\": \"Asset transfer request has been successfully completed\"\n      },\n      \"comment\": \"Transfer Settled\"\n    }\n  ],\n  \"created\": \"2023-10-20T13:02:50.960Z\",\n  \"updated\": \"2023-11-02T00:01:19.340Z\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "5ff339fb-ec45-4721-b0d9-a4f440f68f64",
              "name": "List Transfers",
              "request": {
                "name": "List Transfers",
                "description": {
                  "content": "Lists all of your Transfers across all Accounts. This can be filtered by type of Transfer.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "asset-transfers"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "A status to filter by",
                        "type": "text/plain"
                      },
                      "key": "status",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) A Transfer type to filter by",
                        "type": "text/plain"
                      },
                      "key": "type",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "Maximum number of records to be returned",
                        "type": "text/plain"
                      },
                      "key": "limit",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "Specify an identifier from last API response to go to the next page or prev page",
                        "type": "text/plain"
                      },
                      "key": "offset",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "Go to the next page or prev page",
                        "type": "text/plain"
                      },
                      "key": "direction",
                      "value": "<string>"
                    }
                  ],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "e0c26643-a493-4b38-b19a-fa399bb1e483",
                  "name": "Listing Transfers was successful",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "asset-transfers"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "status",
                          "value": "<string>"
                        },
                        {
                          "key": "type",
                          "value": "<string>"
                        },
                        {
                          "key": "limit",
                          "value": "<string>"
                        },
                        {
                          "key": "offset",
                          "value": "<string>"
                        },
                        {
                          "key": "direction",
                          "value": "<string>"
                        }
                      ],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"data\": [\n    {\n      \"id\": \"grad_ba9522d8-0f3a-43bd-bb16-9efc0ad1a913\",\n      \"source\": \"DWCW001118\",\n      \"destination\": \"DWYE001127\",\n      \"status\": {\n        \"name\": \"SUCCESSFUL\",\n        \"description\": \"Asset transfer request has been successfully completed\"\n      },\n      \"type\": {\n        \"name\": \"TEEN\",\n        \"description\": \"Teen Account Transfer\"\n      },\n      \"partner\": {\n        \"id\": \"25f77a3e-2a4b-48bf-bea2-1b8bcd541621\",\n        \"name\": \"Stark House\"\n      },\n      \"auditDetails\": [\n        {\n          \"timestamp\": \"2023-10-25T16:00:42.126Z\",\n          \"status\": {\n            \"name\": \"STARTED\",\n            \"description\": \"Asset transfer request has been initiated.\"\n          },\n          \"comment\": \"Transfer request has been submitted in queue\"\n        },\n        {\n          \"timestamp\": \"2023-10-25T16:00:42.257Z\",\n          \"status\": {\n            \"name\": \"PENDING\",\n            \"description\": \"Asset transfer request is pending\"\n          },\n          \"comment\": \"Transfer process started\"\n        },\n        {\n          \"timestamp\": \"2023-10-27T21:00:07.959Z\",\n          \"status\": {\n            \"name\": \"ON_HOLD\",\n            \"description\": \"Asset transfer request is on hold.\"\n          },\n          \"comment\": \"Transfer is on hold for DWCW001118. Settlement is not finished yet.\"\n        },\n        {\n          \"timestamp\": \"2023-10-28T14:00:02.453Z\",\n          \"status\": {\n            \"name\": \"SUCCESSFUL\",\n            \"description\": \"Asset transfer request has been successfully completed\"\n          },\n          \"comment\": \"Transfer Completed\"\n        }\n      ],\n      \"created\": \"2023-10-25T16:00:42.126Z\",\n      \"updated\": \"2023-10-28T14:00:02.453Z\"\n    },\n    {\n      \"id\": \"grad_47edac5a-57f0-456a-83ca-128205fcdf3d\",\n      \"source\": \"DWXG000976\",\n      \"destination\": \"DWHZ001105\",\n      \"status\": {\n        \"name\": \"ON_HOLD\",\n        \"description\": \"Asset transfer request is on hold.\"\n      },\n      \"type\": {\n        \"name\": \"TEEN\",\n        \"description\": \"Teen Account Transfer\"\n      },\n      \"partner\": {\n        \"id\": \"25f77a3e-2a4b-48bf-bea2-1b8bcd541621\",\n        \"name\": \"Stark House\"\n      },\n      \"auditDetails\": [\n        {\n          \"timestamp\": \"2023-10-29T04:00:56.167Z\",\n          \"status\": {\n            \"name\": \"STARTED\",\n            \"description\": \"Asset transfer request has been initiated.\"\n          },\n          \"comment\": \"Transfer request has been submitted in queue\"\n        },\n        {\n          \"timestamp\": \"2023-10-29T04:00:56.309Z\",\n          \"status\": {\n            \"name\": \"PENDING\",\n            \"description\": \"Asset transfer request is pending\"\n          },\n          \"comment\": \"Transfer process started\"\n        },\n        {\n          \"timestamp\": \"2023-11-01T21:00:02.207Z\",\n          \"status\": {\n            \"name\": \"ON_HOLD\",\n            \"description\": \"Asset transfer request is on hold.\"\n          },\n          \"comment\": \"Transfer is on hold for DWXG000976. Settlement is not finished yet.\"\n        }\n      ],\n      \"created\": \"2023-10-29T04:00:56.167Z\",\n      \"updated\": \"2023-11-01T21:00:02.207Z\"\n    }\n  ],\n  \"nextPageOffset\": \"25f77a3e-2a4b-48bf-bea2-1b8bcd541621#grad_47edac5a-57f0-456a-83ca-128205fcdf3d#2023-07-28T23:55:34.142Z\",\n  \"prevPageOffset\": \"\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "679ca003-f153-4b79-ad75-d99bce69f1bb",
          "name": "Settlements",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "6afe3e2b-4d57-445a-b703-68d61fb6d51e",
              "name": "List Cashless Reconciliations",
              "request": {
                "name": "List Cashless Reconciliations",
                "description": {
                  "content": "Fetches a list of daily reconciliations for a firm using cashless settlement.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "funding",
                    "reconciliations"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The date and time in which to end at.",
                        "type": "text/plain"
                      },
                      "key": "to",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The date and time in which to start from.",
                        "type": "text/plain"
                      },
                      "key": "from",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "Filters the reconciliations reports by the type of reconciliation.",
                        "type": "text/plain"
                      },
                      "key": "type",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "Filters the reconciliations reports by the status of reconciliation.",
                        "type": "text/plain"
                      },
                      "key": "status",
                      "value": "<string>"
                    }
                  ],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "056f46b7-0cfb-4820-8f31-1e356fee92a1",
                  "name": "Fetching a list of daily reconciliations for a firm was successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "funding",
                        "reconciliations"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "to",
                          "value": "2022-12-25T18:36:40.609Z"
                        },
                        {
                          "key": "from",
                          "value": "2022-12-08T18:36:40.609Z"
                        },
                        {
                          "key": "type",
                          "value": "CRYPTO"
                        },
                        {
                          "key": "status",
                          "value": "APPROVED"
                        }
                      ],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"id\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9_20240417\",\n    \"date\": \"2024-04-17\",\n    \"status\": \"APPROVED\",\n    \"statusComment\": \"Finished processing breakdown\",\n    \"totalAmount\": 12001.01,\n    \"created\": \"2024-04-15T22:28:21.810Z\",\n    \"updated\": \"2024-04-17T22:28:21.810Z\",\n    \"updatedBy\": \"SYSTEM REPORT SERVICE\"\n  },\n  {\n    \"id\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9_20240417\",\n    \"date\": \"2024-04-17\",\n    \"status\": \"APPROVED\",\n    \"statusComment\": \"Finished processing breakdown\",\n    \"totalAmount\": 12001.01,\n    \"created\": \"2024-04-15T22:28:21.810Z\",\n    \"updated\": \"2024-04-17T22:28:21.810Z\",\n    \"updatedBy\": \"INSTANT FUNDING BREAKDOWN JOB\"\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "f4dd49a4-8a12-4b27-b95b-579cbbc75091",
              "name": "Retrieve Cashless Reconciliation",
              "request": {
                "name": "Retrieve Cashless Reconciliation",
                "description": {
                  "content": "Fetches reconciliations details for a firm using cashless settlement.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "funding",
                    "reconciliations",
                    ":reconciliationID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The unique identifier of the reconciliation report.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "reconciliationID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "288db03f-78c1-4c51-ba77-b64c493f5321",
                  "name": "Fetching a firm's reconciliation details was successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "funding",
                        "reconciliations",
                        ":reconciliationID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) The unique identifier of the reconciliation report.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "reconciliationID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9_20240417\",\n  \"date\": \"2024-04-17\",\n  \"status\": \"APPROVED\",\n  \"statusComment\": \"Finished processing breakdown\",\n  \"amounts\": {\n    \"total\": -1263.56,\n    \"purchases\": -1680.07,\n    \"sales\": 416.51,\n    \"dividends\": 0,\n    \"fees\": 0,\n    \"other\": 0\n  },\n  \"transferAmounts\": {\n    \"currency\": \"USD\",\n    \"payablesToDW\": 1263.56,\n    \"receivablesFromDW\": 0\n  },\n  \"reconciliationBreakdown\": {\n    \"JSON\": \"https://d3k101jzh5wilt.cloudfront.net/reconciliation_2e901d48-dd17-42fe-8225-32d2ca6b633e_20190322.json?Policy=eyJTdGF0ddiOiBbeyJSZXNvdXJjZSI6Imh0dHBzOi8vZDNrMTAxanpoNXdpbHQuY2xvdWRmcm9udC5uZXQvcmVjb25jaWxpYXRpb25fMmU5ffdasdamA17ggVl6C40gHkKsr2HLfmjTd9BevcYRPh-QDKA1J~76INZ3nfada4ROS6OUR66A%22\"\n  },\n  \"partnerID\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9\",\n  \"created\": \"2024-04-15T22:28:21.810Z\",\n  \"updated\": \"2024-04-17T22:28:21.810Z\",\n  \"updatedBy\": \"SYSTEM REPORT SERVICE\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "ac3c9f48-cf06-4d20-b369-d1b1e90695ce",
              "name": "Update Cashless Reconciliation",
              "request": {
                "name": "Update Cashless Reconciliation",
                "description": {
                  "content": "Updates a Cashless Reconciliation by reconciliationID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "funding",
                    "reconciliations",
                    ":reconciliationID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "reconciliationID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "PATCH",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"status\": \"<string>\",\n  \"statusComment\": \"<string>\"\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "ae6d1109-048f-4efa-a0e9-a554bbe87649",
                  "name": "Updating the Cashless Reconciliations was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "funding",
                        "reconciliations",
                        ":reconciliationID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "reconciliationID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "PATCH",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"status\": \"SUCCESSFUL\",\n  \"statusComment\": \"Manually approving reconciliation for testing purposes.\"\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9_20240417\",\n  \"date\": \"2024-04-17\",\n  \"status\": \"APPROVED\",\n  \"statusComment\": \"Finished processing breakdown\",\n  \"amounts\": {\n    \"total\": -1263.56,\n    \"purchases\": -1680.07,\n    \"sales\": 416.51,\n    \"dividends\": 0,\n    \"fees\": 0,\n    \"other\": 0\n  },\n  \"transferAmounts\": {\n    \"currency\": \"USD\",\n    \"payablesToDW\": 1263.56,\n    \"receivablesFromDW\": 0\n  },\n  \"reconciliationBreakdown\": {\n    \"JSON\": \"https://d3k101jzh5wilt.cloudfront.net/reconciliation_2e901d48-dd17-42fe-8225-32d2ca6b633e_20190322.json?Policy=eyJTdGF0ddiOiBbeyJSZXNvdXJjZSI6Imh0dHBzOi8vZDNrMTAxanpoNXdpbHQuY2xvdWRmcm9udC5uZXQvcmVjb25jaWxpYXRpb25fMmU5ffdasdamA17ggVl6C40gHkKsr2HLfmjTd9BevcYRPh-QDKA1J~76INZ3nfada4ROS6OUR66A%22\"\n  },\n  \"partnerID\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9\",\n  \"created\": \"2024-04-15T22:28:21.810Z\",\n  \"updated\": \"2024-04-17T22:28:21.810Z\",\n  \"updatedBy\": \"SYSTEM REPORT SERVICE\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "877ec5c7-e5c7-424a-97a7-443368f56df0",
              "name": "Create DVP RVP Report",
              "request": {
                "name": "Create DVP RVP Report",
                "description": {
                  "content": "Creates a job to generate a DVP RVP Report.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "reports",
                    "daily-trade-summary"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "POST",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"tradeDate\": \"<date>\",\n  \"note\": \"<string>\"\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "12a6d016-fbb8-4289-8e41-b3f069c4d301",
                  "name": "Creating the job to generate a DVP/RVP Report was successful",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "reports",
                        "daily-trade-summary"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"tradeDate\": \"<date>\",\n  \"note\": \"Hey! Welcome to DriveWealth Developer Docs!\"\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"bsr_040fb9cc-84e8-4f20-bf09-d398dacd458d.1622745430469_20210604\",\n  \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n  \"accountNo\": \"DWBG000052\",\n  \"tradeDate\": \"yyyy-MM-dd\",\n  \"note\": \"Hey! Welcome to DriveWealth Developer Docs!\",\n  \"partnerID\": \"80f9b672-120d-4b73-9ccv9-42fb3262c4b9\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "210fe7ee-0fd6-457f-888d-3093491e4ec6",
              "name": "List DVP RVP Reports",
              "request": {
                "name": "List DVP RVP Reports",
                "description": {
                  "content": "Lists DVP RVP reports.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "reports",
                    "daily-trade-summary"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "A filter, to filter on the status of the DVP/RVP.",
                        "type": "text/plain"
                      },
                      "key": "status",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "key": "from",
                      "value": "<date>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "key": "to",
                      "value": "<date>"
                    }
                  ],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "fabdf4ee-5de7-466b-aa92-b6060a001679",
                  "name": "Fetching DVP/RVP List was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "reports",
                        "daily-trade-summary"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "status",
                          "value": "Processing"
                        },
                        {
                          "key": "from",
                          "value": "<date>"
                        },
                        {
                          "key": "to",
                          "value": "<date>"
                        }
                      ],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"id\": \"bsr_040fb9cc-84e8-4f20-bf09-d398dacd458d.1622745430469_20210604\",\n    \"tradeDate\": \"yyyy-MM-dd\",\n    \"status\": \"SUCCESSFUL\",\n    \"note\": \"Hey! Welcome to DriveWealth Developer Docs!\",\n    \"partnerID\": \"80f9b672-120d-4b73-9ccv9-42fb3262c4b9\",\n    \"created\": \"2022-12-11T22:28:21.810Z\",\n    \"updated\": \"2022-12-11T22:28:21.810Z\",\n    \"updatedBy\": \"SYSTEM REPORT SERVICE\",\n    \"source\": \"MANUAL\"\n  },\n  {\n    \"id\": \"bsr_040fb9cc-84e8-4f20-bf09-d398dacd458d.1622745430469_20210604\",\n    \"tradeDate\": \"yyyy-MM-dd\",\n    \"status\": \"SUCCESSFUL\",\n    \"note\": \"Hey! Welcome to DriveWealth Developer Docs!\",\n    \"partnerID\": \"80f9b672-120d-4b73-9ccv9-42fb3262c4b9\",\n    \"created\": \"2022-12-11T22:28:21.810Z\",\n    \"updated\": \"2022-12-11T22:28:21.810Z\",\n    \"updatedBy\": \"INSTANT FUNDING BREAKDOWN JOB\",\n    \"source\": \"MANUAL\"\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "0decd729-0802-4afc-bc56-56ea9ae36e5b",
              "name": "Retrieve DVP RVP",
              "request": {
                "name": "Retrieve DVP RVP",
                "description": {
                  "content": "Retrieves a DVP RVP by reportID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "reports",
                    "daily-trade-summary",
                    ":reportID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "reportID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "4b3f301f-2b4f-41f2-8110-1fb1e98bfaaf",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "reports",
                        "daily-trade-summary",
                        ":reportID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        },
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "reportID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"bsr_040fb9cc-84e8-4f20-bf09-d398dacd458d.1622745430469_20210604\",\n  \"tradeDate\": \"yyyy-MM-dd\",\n  \"status\": \"SUCCESSFUL\",\n  \"note\": \"Hey! Welcome to DriveWealth Developer Docs!\",\n  \"partnerID\": \"80f9b672-120d-4b73-9ccv9-42fb3262c4b9\",\n  \"created\": \"2022-12-11T22:28:21.810Z\",\n  \"updated\": \"2022-12-11T22:28:21.810Z\",\n  \"updatedBy\": \"INSTANT FUNDING BREAKDOWN JOB\",\n  \"source\": \"MANUAL\",\n  \"amount\": {\n    \"totalBuy\": {\n      \"quantity\": 10.71358941,\n      \"notional\": 144.26,\n      \"orders\": 30\n    },\n    \"totalSell\": {\n      \"quantity\": 0,\n      \"notional\": 0,\n      \"orders\": 0\n    }\n  },\n  \"breakdownJson\": \"https://du2c4wzqz90h1.cloudfront.net/buySellTradesReport....\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "a2812a3c-363c-4a58-9c93-213a4726c30b",
              "name": "Retrieve Settlements",
              "request": {
                "name": "Retrieve Settlements",
                "description": {
                  "content": "Retrieves a list of Settlements.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "settlements"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The date to start from.",
                        "type": "text/plain"
                      },
                      "key": "from",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The date to end at.",
                        "type": "text/plain"
                      },
                      "key": "to",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "Filters, the settlements by the status.",
                        "type": "text/plain"
                      },
                      "key": "status",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "Filters, the settlements by the settlement profile.",
                        "type": "text/plain"
                      },
                      "key": "settlementProfileID",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The number of items to return.",
                        "type": "text/plain"
                      },
                      "key": "limit",
                      "value": "50"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "Used for pagination. Set this to the first/last id value of your payload to get the prev/next page of results respectively.",
                        "type": "text/plain"
                      },
                      "key": "offset",
                      "value": ""
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The direction of the pagination.",
                        "type": "text/plain"
                      },
                      "key": "direction",
                      "value": "<string>"
                    }
                  ],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "1eb2e509-dd59-4063-ac79-1bb2c5e6be37",
                  "name": "Retrieving a list of Settlements was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "settlements"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "from",
                          "value": "2022-12-08"
                        },
                        {
                          "key": "to",
                          "value": "2022-12-25"
                        },
                        {
                          "key": "status",
                          "value": "PENDING"
                        },
                        {
                          "key": "settlementProfileID",
                          "value": "settlement-profile-bank-account-1"
                        },
                        {
                          "key": "limit",
                          "value": "50"
                        },
                        {
                          "key": "offset",
                          "value": ""
                        },
                        {
                          "key": "direction",
                          "value": "<string>"
                        }
                      ],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"pageSize\": 1,\n  \"limit\": 50,\n  \"settlements\": [\n    {\n      \"id\": \"sett_63ccb073-a7b6-4b33-af77-5baec5cc4494_settle-profile-usa_20221224\",\n      \"settlementDate\": \"2022-12-25\",\n      \"partnerID\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9\",\n      \"status\": \"PENDING\",\n      \"totalAmount\": -14250,\n      \"createdAt\": \"2022-12-11T22:28:21.810Z\",\n      \"updatedAt\": \"2022-12-11T22:28:21.810Z\",\n      \"settlementProfileID\": \"settlement-profile-bank-account-1\"\n    },\n    {\n      \"id\": \"sett_63ccb073-a7b6-4b33-af77-5baec5cc4494_settle-profile-usa_20221224\",\n      \"settlementDate\": \"2022-12-25\",\n      \"partnerID\": \"80f9b672-120d-4b73-9cc9-42fb3262c4b9\",\n      \"status\": \"PENDING\",\n      \"totalAmount\": -14250,\n      \"createdAt\": \"2022-12-11T22:28:21.810Z\",\n      \"updatedAt\": \"2022-12-11T22:28:21.810Z\",\n      \"settlementProfileID\": \"settlement-profile-bank-account-1\"\n    }\n  ]\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "73904405-8060-4ecd-98d3-98581a8a7a26",
              "name": "Retrieve Settlement",
              "request": {
                "name": "Retrieve Settlement",
                "description": {
                  "content": "Retrieves Settlement by settlementID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "settlements",
                    ":settlementID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "settlementID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "469c7f5d-7868-4bbc-a578-435ddcc801d1",
                  "name": "Retrieving Settlement by settlementID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "settlements",
                        ":settlementID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "settlementID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"sett_63ccb073-a7b6-4b33-af77-5baec5cc4494_settle-profile-usa_20221224\",\n  \"settlementDate\": \"2022-12-25\",\n  \"status\": \"PENDING\",\n  \"statusComment\": \"Finished processing breakdown\",\n  \"amount\": {\n    \"total\": 5000.45,\n    \"credits\": 6000.45,\n    \"debits\": -1000\n  },\n  \"breakdownReport\": \"https://du2c4wzqz90h1.cloudfront.net/singleSettlementReport....\",\n  \"partnerID\": \"80f9b672-120d-4b73-9ccv9-42fb3262c4b9\",\n  \"settlementProfileID\": \"settlement-profile-bank-account-1\",\n  \"updatedBy\": \"SYSTEM REPORT SERVICE\",\n  \"createdAt\": \"2022-12-11T22:28:21.810Z\",\n  \"updatedAt\": \"2022-12-11T22:28:21.810Z\"\n}",
                  "cookie": []
                },
                {
                  "_": {
                    "postman_previewlanguage": "text"
                  },
                  "id": "3555caa6-1276-48cd-8dab-3d4e39593849",
                  "name": "The settlement for given settlementID doesn't exist.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "settlements",
                        ":settlementID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "settlementID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "Not Found",
                  "code": 404,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "text/plain"
                    }
                  ],
                  "body": "",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "c771c518-9de6-4a55-95a9-1bfa86f7e7ef",
          "name": "Subscriptions",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [],
          "event": []
        }
      ],
      "event": []
    },
    {
      "id": "b75435b7-ca69-4a49-b792-8942ac88ee02",
      "name": "Account Management APIs",
      "item": [
        {
          "id": "a97a9ccf-fe6d-412b-a413-42a4f1f011b1",
          "name": "Violations",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "c561f3d4-eb6d-438a-969f-682f35a504e2",
              "name": "Retrieve Account Violations Summary",
              "request": {
                "name": "Retrieve Account Violations Summary",
                "description": {
                  "content": "Retrives Account Violations Summary details by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "summary",
                    "violations"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "22d5a9aa-3208-4fdc-b4b7-a77b8efd9705",
                  "name": "Retrieving an Account Violations Summary details by accountID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "summary",
                        "violations"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n  \"accountNo\": \"DWBG000052\",\n  \"tradingType\": \"CASH\",\n  \"updated\": \"2017-06-16T15:35:30.617Z\",\n  \"violations\": {\n    \"goodFaithViolations\": {\n      \"count\": 0\n    },\n    \"patternDayTrades\": {\n      \"count\": 0\n    },\n    \"details\": \"/back-office/accounts/b5421694-65c6-4e48-9f8f-d90596e2f471.1616427127842/violations\"\n  }\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "6e241d18-ed36-4067-82f7-cd14ab64ac6d",
              "name": "List Account Violations",
              "request": {
                "name": "List Account Violations",
                "description": {
                  "content": "Retrives a list of Account Violations by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "violations"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "ff0f0a76-f7df-42b4-b4aa-3c25164e959b",
                  "name": "Retrieving a list of Account Violations by accountID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "violations"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"goodFaithViolations\": {\n    \"count\": 0\n  },\n  \"patternDayTrades\": [\n    {\n      \"id\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n      \"symbol\": \"MS\",\n      \"qty\": 0.7219,\n      \"amount\": 100,\n      \"side\": \"B\",\n      \"createdWhen\": \"2022-12-11T22:28:21.810Z\",\n      \"orderID\": \"IC.0e352bb7-9869-4233-9861-9673544efedd\",\n      \"orderNo\": \"ICDU023727\",\n      \"violationSells\": [\n        {\n          \"qty\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"amount\": 20,\n          \"createdWhen\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"orderID\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"orderNo\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"side\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          }\n        },\n        {\n          \"qty\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"amount\": 20,\n          \"createdWhen\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"orderID\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"orderNo\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"side\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          }\n        }\n      ],\n      \"legacyGoodFaithViolations\": 0,\n      \"message\": \"This transaction resulted in your third Pattern Day Trade.  Note that pending orders (such as limits) may trigger a 4th Pattern Day Trade.  If you have 4 or more day trades in a 5 day period, your account will be designated as a Pattern Day Trader and must maintain equity of at least $25,000.  Failure to do so will put your account on 90-Restriction. You will receive an email notification with more details.\"\n    },\n    {\n      \"id\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n      \"symbol\": \"MS\",\n      \"qty\": 0.7219,\n      \"amount\": 100,\n      \"side\": \"B\",\n      \"createdWhen\": \"2022-12-11T22:28:21.810Z\",\n      \"orderID\": \"IC.0e352bb7-9869-4233-9861-9673544efedd\",\n      \"orderNo\": \"ICDU023727\",\n      \"violationSells\": [\n        {\n          \"qty\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"amount\": 20,\n          \"createdWhen\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"orderID\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"orderNo\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"side\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          }\n        },\n        {\n          \"qty\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"amount\": 20,\n          \"createdWhen\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"orderID\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"orderNo\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"side\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          }\n        }\n      ],\n      \"legacyGoodFaithViolations\": 0,\n      \"message\": \"This transaction resulted in your third Pattern Day Trade.  Note that pending orders (such as limits) may trigger a 4th Pattern Day Trade.  If you have 4 or more day trades in a 5 day period, your account will be designated as a Pattern Day Trader and must maintain equity of at least $25,000.  Failure to do so will put your account on 90-Restriction. You will receive an email notification with more details.\"\n    }\n  ],\n  \"accountEquityBreakdown\": {\n    \"longMarketValue\": 30000,\n    \"debitBalance\": 2000,\n    \"accountEquity\": 28000\n  }\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "0600e702-460d-492f-a1d1-2585a7d0cf61",
          "name": "Statements",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "88c822db-8690-4b67-b1bd-1e42f70af63f",
              "name": "List Account Statements",
              "request": {
                "name": "List Account Statements",
                "description": {
                  "content": "Retrives a list of Account Statements by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "statements"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "c5290a81-3eaa-4199-be3b-fffb6c55c739",
                  "name": "Retrieving a list of Account Statements by accountID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "statements"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"displayName\": \"Apr 28, 2017 Statement\",\n    \"fileKey\": \"2017042802\"\n  },\n  {\n    \"displayName\": \"Apr 28, 2017 Statement\",\n    \"fileKey\": \"2017042802\"\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "f6c6c11a-174a-417d-ab6f-3e0128d2b54c",
              "name": "List Account Tax Statements",
              "request": {
                "name": "List Account Tax Statements",
                "description": {
                  "content": "Retrieves a list of Account Tax Statements by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "taxforms"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "The date to start the filter.",
                        "type": "text/plain"
                      },
                      "key": "from",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The date to end the filter.",
                        "type": "text/plain"
                      },
                      "key": "to",
                      "value": "<string>"
                    }
                  ],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "62973f96-886a-4ad4-8726-2138957a80f6",
                  "name": "Retrieving a list of  Account Tax Statements by accountID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "taxforms"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "from",
                          "value": "2022-06-16"
                        },
                        {
                          "key": "to",
                          "value": "2022-07-16"
                        }
                      ],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"displayName\": \"2015 Tax Year 1099-B\",\n    \"fileKey\": \"2015123103\"\n  },\n  {\n    \"displayName\": \"2015 Tax Year 1099-B\",\n    \"fileKey\": \"2015123103\"\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "91cee3c6-4e70-4baf-a198-5334aab96f7f",
              "name": "List Account Trade Confirmations",
              "request": {
                "name": "List Account Trade Confirmations",
                "description": {
                  "content": "Retrieves a list of Account Trade Confirmations by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "confirms"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "Filter, the date from which to start the search.",
                        "type": "text/plain"
                      },
                      "key": "from",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "Filter, the date to which to end the search.",
                        "type": "text/plain"
                      },
                      "key": "to",
                      "value": "<string>"
                    }
                  ],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "1df429d6-24f2-411f-94b4-5f8915cbcff2",
                  "name": "Retrieving a list of Account Trade Confirmations by accountID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "confirms"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "from",
                          "value": "2018-09-18"
                        },
                        {
                          "key": "to",
                          "value": "2019-09-18"
                        }
                      ],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"displayName\": \"Jun 02, 2017 Trade Confirm\",\n    \"fileKey\": \"2017060201\"\n  },\n  {\n    \"displayName\": \"Jun 02, 2017 Trade Confirm\",\n    \"fileKey\": \"2017060201\"\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "b57a0e66-1933-4d3a-bedd-01e82bb828b6",
              "name": "Retrieve Statement",
              "request": {
                "name": "Retrieve Statement",
                "description": {
                  "content": "Retrieves an Account Statement (Monthly, Trade Confirms, Tax Forms, etc.) by accountID and fileKey.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "statements",
                    ":accountID",
                    ":fileKey"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "fileKey"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "965edea0-252e-465a-9b34-f9788068db5f",
                  "name": "Retrieving an Account Statement was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "statements",
                        ":accountID",
                        ":fileKey"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        },
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "fileKey"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n  \"url\": \"https://dzb6emi8pracf.cloudfront.net/5a013513-8af1-4078-be75-36a5250953f7.1488219178676/Stmt_DRVW_001_DWJM000019_Apr2017.pdf?Policy=eyJTdGF0ZW1lbnQiOiBbeyJSZXNvdXJjZSI6Imh0dHBzOi8vZHpiNmVtaThwcmFjZi5jbG91ZGZyb250Lm5ldC81YTAxMzUxMy04YWYxLTQwNzgtYmU3NS0zNmE1MjUwOTUzZjcuMTQ4ODIxOTE3ODY3Ni9TdG10X0RSVldfMDAxX0RXSk0wMDAwMTlfQXByMjAxNy5wZGYiLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE0OTk3MTc1NDV9LCJJcEFkZHJlc3MiOnsiQVdTOlNvdXJjZUlwIjoiMC4wLjAuMC8wIn19fV19&Signature=UWZRPku4IWoqkp4fyQ179auFVrImZUYDXswjjO-zPGW9-XKno3-TG9O2OHxWG-j7NfEHMXtZbCha~lQwpjt~g58YpL1NYk9xhlp7~HR-skC3J3W8GFVWxbR5TQUXPFOdU-KNwYlTnlE1Wr81nUyoNWrrF-8afyiHVnfm2w35GpZavAKhOiKNDHn7kTorQz3rbkYDks9u1CGPU7TCeZ-GzupVqsUN7xDOxPUnH0KCVGY86PT8bEpPkhpc3jNmtLnB~WB3YdrFg0bSbrbU4M-sVyp49AqK~xq5uDu3Bx22vdyJlKUClEsVvKhQLOArkpMdHYwyPZC~Kz85sroGqnP3oQ__&Key-Pair-Id=APKAJP3MFGZ6DRA4CW4Q\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "4be43026-a04d-42ab-8642-7d2d0b93bfc5",
          "name": "Beneficiaries",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "b250a0ca-81f7-4f49-9109-2d7b609b677a",
              "name": "Create Account Beneficiaries",
              "request": {
                "name": "Create Account Beneficiaries",
                "description": {
                  "content": "Creates an Account Beneficiary by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "beneficiaries"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "POST",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"primary\": [\n    {\n      \"type\": \"<string>\",\n      \"name\": \"<string>\",\n      \"percentage\": \"<number>\",\n      \"email\": \"<string>\",\n      \"formationDate\": \"<string>\",\n      \"primaryContact\": \"<string>\",\n      \"phone\": \"<string>\",\n      \"created\": \"<string>\"\n    },\n    {\n      \"type\": \"<string>\",\n      \"name\": \"<string>\",\n      \"percentage\": \"<number>\",\n      \"email\": \"<string>\",\n      \"formationDate\": \"<string>\",\n      \"primaryContact\": \"<string>\",\n      \"phone\": \"<string>\",\n      \"created\": \"<string>\"\n    }\n  ],\n  \"contingent\": [\n    {\n      \"type\": \"<string>\",\n      \"name\": \"<string>\",\n      \"percentage\": \"<number>\",\n      \"email\": \"<string>\",\n      \"formationDate\": \"<string>\",\n      \"primaryContact\": \"<string>\",\n      \"phone\": \"<string>\",\n      \"created\": \"<string>\"\n    },\n    {\n      \"type\": \"<string>\",\n      \"name\": \"<string>\",\n      \"percentage\": \"<number>\",\n      \"email\": \"<string>\",\n      \"formationDate\": \"<string>\",\n      \"primaryContact\": \"<string>\",\n      \"phone\": \"<string>\",\n      \"created\": \"<string>\"\n    }\n  ]\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "56a6dfb3-f8a9-4607-b93f-d602d3587ba6",
                  "name": "Creating an Account Beneficiary was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "beneficiaries"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"primary\": [\n    {\n      \"type\": \"ENTITY\",\n      \"name\": \"Tom Ace\",\n      \"percentage\": \"<number>\",\n      \"email\": \"tom@ac.com\",\n      \"formationDate\": \"2010-10-25\",\n      \"primaryContact\": \"5512478089\",\n      \"phone\": \"4153647890\",\n      \"created\": \"2022-12-29T18:32:15.533Z\"\n    },\n    {\n      \"type\": \"ENTITY\",\n      \"name\": \"Tom Ace\",\n      \"percentage\": \"<number>\",\n      \"email\": \"tom@ac.com\",\n      \"formationDate\": \"2010-10-25\",\n      \"primaryContact\": \"5512478089\",\n      \"phone\": \"4153647890\",\n      \"created\": \"2022-12-29T18:32:15.533Z\"\n    }\n  ],\n  \"contingent\": [\n    {\n      \"type\": \"ENTITY\",\n      \"name\": \"Tom Ace\",\n      \"percentage\": \"<number>\",\n      \"email\": \"tom@ac.com\",\n      \"formationDate\": \"2010-10-25\",\n      \"primaryContact\": \"5512478089\",\n      \"phone\": \"4153647890\",\n      \"created\": \"2022-12-29T18:32:15.533Z\"\n    },\n    {\n      \"type\": \"ENTITY\",\n      \"name\": \"Tom Ace\",\n      \"percentage\": \"<number>\",\n      \"email\": \"tom@ac.com\",\n      \"formationDate\": \"2010-10-25\",\n      \"primaryContact\": \"5512478089\",\n      \"phone\": \"4153647890\",\n      \"created\": \"2022-12-29T18:32:15.533Z\"\n    }\n  ]\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"primary\": [\n    {\n      \"type\": \"ENTITY\",\n      \"name\": \"Tom Ace\",\n      \"percentage\": \"<number>\",\n      \"email\": \"tom@ac.com\",\n      \"formationDate\": \"2010-10-25\",\n      \"primaryContact\": \"5512478089\",\n      \"phone\": \"4153647890\",\n      \"created\": \"2022-12-29T18:32:15.533Z\"\n    },\n    {\n      \"type\": \"ENTITY\",\n      \"name\": \"Tom Ace\",\n      \"percentage\": \"<number>\",\n      \"email\": \"tom@ac.com\",\n      \"formationDate\": \"2010-10-25\",\n      \"primaryContact\": \"5512478089\",\n      \"phone\": \"4153647890\",\n      \"created\": \"2022-12-29T18:32:15.533Z\"\n    }\n  ],\n  \"contingent\": [\n    {\n      \"type\": \"ENTITY\",\n      \"name\": \"Tom Ace\",\n      \"percentage\": \"<number>\",\n      \"email\": \"tom@ac.com\",\n      \"formationDate\": \"2010-10-25\",\n      \"primaryContact\": \"5512478089\",\n      \"phone\": \"4153647890\",\n      \"created\": \"2022-12-29T18:32:15.533Z\"\n    },\n    {\n      \"type\": \"ENTITY\",\n      \"name\": \"Tom Ace\",\n      \"percentage\": \"<number>\",\n      \"email\": \"tom@ac.com\",\n      \"formationDate\": \"2010-10-25\",\n      \"primaryContact\": \"5512478089\",\n      \"phone\": \"4153647890\",\n      \"created\": \"2022-12-29T18:32:15.533Z\"\n    }\n  ]\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "4c18b9f8-70c2-4aa2-9f25-950c5fcc1a03",
              "name": "Retrieve Account Beneficiaries",
              "request": {
                "name": "Retrieve Account Beneficiaries",
                "description": {
                  "content": "Retrieves a list of Account Beneficiaries by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "beneficiaries"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "dfa96334-4a9c-4be9-823f-d0bf98fb641f",
                  "name": "Retrieving a list of Account Beneficiaries was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "beneficiaries"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"primary\": [\n    {\n      \"type\": \"ENTITY\",\n      \"name\": \"Tom Ace\",\n      \"percentage\": \"<number>\",\n      \"email\": \"tom@ac.com\",\n      \"formationDate\": \"2010-10-25\",\n      \"primaryContact\": \"5512478089\",\n      \"phone\": \"4153647890\",\n      \"created\": \"2022-12-29T18:32:15.533Z\"\n    },\n    {\n      \"type\": \"ENTITY\",\n      \"name\": \"Tom Ace\",\n      \"percentage\": \"<number>\",\n      \"email\": \"tom@ac.com\",\n      \"formationDate\": \"2010-10-25\",\n      \"primaryContact\": \"5512478089\",\n      \"phone\": \"4153647890\",\n      \"created\": \"2022-12-29T18:32:15.533Z\"\n    }\n  ],\n  \"contingent\": [\n    {\n      \"type\": \"ENTITY\",\n      \"name\": \"Tom Ace\",\n      \"percentage\": \"<number>\",\n      \"email\": \"tom@ac.com\",\n      \"formationDate\": \"2010-10-25\",\n      \"primaryContact\": \"5512478089\",\n      \"phone\": \"4153647890\",\n      \"created\": \"2022-12-29T18:32:15.533Z\"\n    },\n    {\n      \"type\": \"ENTITY\",\n      \"name\": \"Tom Ace\",\n      \"percentage\": \"<number>\",\n      \"email\": \"tom@ac.com\",\n      \"formationDate\": \"2010-10-25\",\n      \"primaryContact\": \"5512478089\",\n      \"phone\": \"4153647890\",\n      \"created\": \"2022-12-29T18:32:15.533Z\"\n    }\n  ]\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "e0a0178e-d74a-476f-82c2-1c511f68cb87",
              "name": "Delete Account Beneficiaries",
              "request": {
                "name": "Delete Account Beneficiaries",
                "description": {
                  "content": "Removes all Accounts Beneficiaries by accountID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "accounts",
                    ":accountID",
                    "beneficiaries"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) ",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "accountID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "DELETE"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "text"
                  },
                  "id": "6a55d34e-a735-4ad2-bfdd-c124a8fa1f24",
                  "name": "Removing all Account Beneficiaries was Accepted.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "accounts",
                        ":accountID",
                        "beneficiaries"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) ",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "accountID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "DELETE",
                    "body": {}
                  },
                  "status": "Accepted",
                  "code": 202,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "text/plain"
                    }
                  ],
                  "body": "",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "9fd9c089-df15-4bc8-86b0-1377fb6f5741",
          "name": "Physical Documents",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "952c6c2d-3bc8-41bd-8476-bff7907873a2",
              "name": "Upload Physical Document",
              "request": {
                "name": "Upload Physical Document",
                "description": {
                  "content": "Uploads a Physical Document.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "documents"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "POST",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"userID\": \"<string>\",\n  \"type\": \"<string>\",\n  \"document\": \"<string>\",\n  \"side\": \"<string>\"\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "e6d3848c-7288-496a-926a-159f7c186f69",
                  "name": "Uploading a Physical Document was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "documents"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"userID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n  \"type\": \"DRIVER_LICENSE\",\n  \"document\": \"data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAASABIAAD/4QCMR\",\n  \"side\": \"FRONT\"\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"532e1b7d-09fd-4a1b-956f-d4e91ad71b4f\",\n  \"type\": \"DRIVER_LICENSE\",\n  \"status\": {\n    \"name\": \"NOT_SUBMITTED\",\n    \"description\": \"Document has not been submitted for approval.\"\n  },\n  \"side\": \"FRONT\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "59d318bb-f0f7-463d-95a6-7d83c59de4f4",
              "name": "Retrieve Physical Document URL",
              "request": {
                "name": "Retrieve Physical Document URL",
                "description": {
                  "content": "Retrieves a Physical Document by documentID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "documents",
                    ":documentID",
                    "url"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The unique identifier of the document.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "documentID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "8e0db9f6-c6c7-43d6-98ac-418c7975b72d",
                  "name": "Retrieving a Physical Document URL by documentID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "documents",
                        ":documentID",
                        "url"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) The unique identifier of the document.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "documentID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "Created",
                  "code": 201,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"url\": \"https://dzb6emi8pracf.cloudfront.net/5a013513-8af1-4078-be75-36a5250953f7.1488219178676/Stmt_DRVW_001_DWJM000019_Apr2017.pdf?Policy=eyJTdGF0ZW1lbnQiOiBbeyJSZXNvdXJjZSI6Imh0dHBzOi8vZHpiNmVtaThwcmFjZi5jbG91ZGZyb250Lm5ldC81YTAxMzUxMy04YWYxLTQwNzgtYmU3NS0zNmE1MjUwOTUzZjcuMTQ4ODIxOTE3ODY3Ni9TdG10X0RSVldfMDAxX0RXSk0wMDAwMTlfQXByMjAxNy5wZGYiLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE0OTk3MTc1NDV9LCJJcEFkZHJlc3MiOnsiQVdTOlNvdXJjZUlwIjoiMC4wLjAuMC8wIn19fV19&Signature=UWZRPku4IWoqkp4fyQ179auFVrImZUYDXswjjO-zPGW9-XKno3-TG9O2OHxWG-j7NfEHMXtZbCha~lQwpjt~g58YpL1NYk9xhlp7~HR-skC3J3W8GFVWxbR5TQUXPFOdU-KNwYlTnlE1Wr81nUyoNWrrF-8afyiHVnfm2w35GpZavAKhOiKNDHn7kTorQz3rbkYDks9u1CGPU7TCeZ-GzupVqsUN7xDOxPUnH0KCVGY86PT8bEpPkhpc3jNmtLnB~WB3YdrFg0bSbrbU4M-sVyp49AqK~xq5uDu3Bx22vdyJlKUClEsVvKhQLOArkpMdHYwyPZC~Kz85sroGqnP3oQ__&Key-Pair-Id=APKAJP3MFGZ6DRA4CW4Q\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "fccd296d-b2c3-4903-a487-e054977f69c3",
              "name": "List User Physical Documents",
              "request": {
                "name": "List User Physical Documents",
                "description": {
                  "content": "Retrieves a list of Users Physical Documents by userID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "users",
                    ":userID",
                    "documents"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The User's unique identifier.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "userID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "33df5003-c2db-44af-a75f-48c1ff96e2ea",
                  "name": "Retrieving a list of Users Physical Documents by userID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "users",
                        ":userID",
                        "documents"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) The User's unique identifier.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "userID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"id\": \"532e1b7d-09fd-4a1b-956f-d4e91ad71b4f\",\n    \"type\": {\n      \"name\": \"DRIVER_LICENSE\",\n      \"description\": \"Driver License\"\n    },\n    \"status\": {\n      \"name\": \"NOT_SUBMITTED\",\n      \"description\": \"The document has not been submitted for approval.\"\n    }\n  },\n  {\n    \"id\": \"532e1b7d-09fd-4a1b-956f-d4e91ad71b4f\",\n    \"type\": {\n      \"name\": \"DRIVER_LICENSE\",\n      \"description\": \"Driver License\"\n    },\n    \"status\": {\n      \"name\": \"NOT_SUBMITTED\",\n      \"description\": \"The document has not been submitted for approval.\"\n    }\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        }
      ],
      "event": []
    },
    {
      "id": "30b10429-eaa5-4993-9d2d-d49d5c1d41be",
      "name": "Advisor APIs",
      "item": [
        {
          "id": "5d78435b-d5be-4456-a3fb-586bb91366c2",
          "name": "Trade Allocations",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "2e611d4f-ce3a-4cb0-b92e-389a859fb40a",
              "name": "Create Trade Allocation",
              "request": {
                "name": "Create Trade Allocation",
                "description": {
                  "content": "Create a Trade Allocation.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "managed",
                    "allocations"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "POST",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"userID\": \"<string>\",\n  \"orders\": [\n    {\n      \"orderID\": \"<string>\",\n      \"allocations\": [\n        {\n          \"accountID\": \"<string>\",\n          \"accountNo\": \"<string>\",\n          \"qty\": \"<string>\",\n          \"useClientFunds\": \"<boolean>\",\n          \"comment\": \"<string>\"\n        },\n        {\n          \"accountID\": \"<string>\",\n          \"accountNo\": \"<string>\",\n          \"qty\": \"<string>\",\n          \"useClientFunds\": \"<boolean>\",\n          \"comment\": \"<string>\"\n        }\n      ]\n    },\n    {\n      \"orderID\": \"<string>\",\n      \"allocations\": [\n        {\n          \"accountID\": \"<string>\",\n          \"accountNo\": \"<string>\",\n          \"qty\": \"<string>\",\n          \"useClientFunds\": \"<boolean>\",\n          \"comment\": \"<string>\"\n        },\n        {\n          \"accountID\": \"<string>\",\n          \"accountNo\": \"<string>\",\n          \"qty\": \"<string>\",\n          \"useClientFunds\": \"<boolean>\",\n          \"comment\": \"<string>\"\n        }\n      ]\n    }\n  ],\n  \"clientListID\": \"<string>\",\n  \"note\": \"<string>\"\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "cafa3cf0-f07d-40ac-bb87-de7241b7c91d",
                  "name": "Creating a Trade Allocation was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "managed",
                        "allocations"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"userID\": \"66304da9-3h6f-2234-935f-ac6b7933d706\",\n  \"orders\": [\n    {\n      \"orderID\": \"JL.562f3719-7c8f-50ee-b234-db7775715a99\",\n      \"allocations\": [\n        {\n          \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n          \"accountNo\": \"ZYXC000008\",\n          \"qty\": \"27\",\n          \"useClientFunds\": true,\n          \"comment\": \"Suds boapi test to 1st\"\n        },\n        {\n          \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n          \"accountNo\": \"ZYXC000008\",\n          \"qty\": \"27\",\n          \"useClientFunds\": true,\n          \"comment\": \"Suds boapi test to 1st\"\n        }\n      ]\n    },\n    {\n      \"orderID\": \"JL.562f3719-7c8f-50ee-b234-db7775715a99\",\n      \"allocations\": [\n        {\n          \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n          \"accountNo\": \"ZYXC000008\",\n          \"qty\": \"27\",\n          \"useClientFunds\": true,\n          \"comment\": \"Suds boapi test to 1st\"\n        },\n        {\n          \"accountID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932.1407775317759\",\n          \"accountNo\": \"ZYXC000008\",\n          \"qty\": \"27\",\n          \"useClientFunds\": true,\n          \"comment\": \"Suds boapi test to 1st\"\n        }\n      ]\n    }\n  ],\n  \"clientListID\": \"SUMS_CUSTOM_ALLOCATION_TEST\",\n  \"note\": \"Allocating via api allocation test\"\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"JL.allocation.SomeRIACompany.9d6def3b-14d7-4934-8a64-57d443e67ce6\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "069dce00-078f-4a29-9343-5bec2b64d63d",
              "name": "Retrieve Trade Allocation",
              "request": {
                "name": "Retrieve Trade Allocation",
                "description": {
                  "content": "Retrieves Trade Allocation by allocationID.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "managed",
                    "allocations",
                    ":allocationID"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The unique identifier returned when a Trade Allocation request is made.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "allocationID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "8b44f8f3-1448-49b7-aff9-ed171981bc40",
                  "name": "Retrieving Trade Allocation by allocationID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "managed",
                        "allocations",
                        ":allocationID"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) The unique identifier returned when a Trade Allocation request is made.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "allocationID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"JL.allocation.SomeRIACompany.9d6def3b-14d7-4934-8a64-57d443e67ce6\",\n  \"status\": \"COMPLETE\",\n  \"clientListID\": \"SUMS_CUSTOM_ALLOCATION_TEST\",\n  \"accountID\": \"66304da9-3d6f-4253-935f-ac6b7933d701.1619201263789\",\n  \"accountNo\": \"ZYXB000008\",\n  \"createdWhen\": \"2022-12-22T16:04:46.724Z\",\n  \"allocations\": [\n    {\n      \"accountID\": \"743a1018-e292-449c-a43f-58d657990db0.1671689261882\",\n      \"accountNo\": \"ZYXC000008\",\n      \"status\": \"FILLED\",\n      \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n      \"symbol\": \"MS\",\n      \"side\": \"B\",\n      \"clientComment\": \"Foo test allocation\",\n      \"qtyRequested\": 10,\n      \"qtyAllocated\": 10,\n      \"avgPx\": 126.52,\n      \"fees\": {\n        \"total\": 44697896.89575598,\n        \"sec\": -42643792.68310616,\n        \"taf\": -53740920.29777118,\n        \"commission\": 20937383.721056774,\n        \"other\": -3641470.0688801855\n      }\n    },\n    {\n      \"accountID\": \"743a1018-e292-449c-a43f-58d657990db0.1671689261882\",\n      \"accountNo\": \"ZYXC000008\",\n      \"status\": \"FILLED\",\n      \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n      \"symbol\": \"MS\",\n      \"side\": \"B\",\n      \"clientComment\": \"Foo test allocation\",\n      \"qtyRequested\": 10,\n      \"qtyAllocated\": 10,\n      \"avgPx\": 126.52,\n      \"fees\": {\n        \"total\": -44790690.29855802,\n        \"sec\": 9804145.655475423,\n        \"taf\": 56087818.68556103,\n        \"commission\": -9454732.84472759,\n        \"other\": 99685539.48233655\n      }\n    }\n  ],\n  \"comment\": \"All allocated and accounted for. 1::1::0 client note[allocating via bo api 1st allocation test]. timeMs=423 ratePerSec=2.36 msPerItem=423.00\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "6c876383-258a-417e-8a9e-c0ca096f606e",
              "name": "List Trade Allocations by Advisor",
              "request": {
                "name": "List Trade Allocations by Advisor",
                "description": {
                  "content": "Fetches a list of an User's allocations.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "users",
                    ":userID",
                    "managed",
                    "allocations"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The User's unique identifier.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "userID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "9154ec48-7d79-42a3-b3f6-b3d6abb11110",
                  "name": "Fetching A List Of A User's Allocation was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "users",
                        ":userID",
                        "managed",
                        "allocations"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) The User's unique identifier.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "userID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"id\": \"JF.allocation.TendiesTradingCo.e61f512a-ed9c-4047-9ccf-224a5864158d\",\n    \"clientListID\": \"Hey! Welcome to DriveWealth Developer Docs!\",\n    \"status\": \"NEW\",\n    \"allocationsRequested\": 500,\n    \"allocationsCompleted\": 25,\n    \"unallocatedNotional\": 5320,\n    \"unallocatedQuantity\": 302,\n    \"comment\": \"All allocated and accounted for. 1::1::0 client note[empty], . timeMs=667 ratePerSec=1.50 msPerItem=667.00\",\n    \"createdWhen\": \"2022-12-22T16:04:46.724Z\"\n  },\n  {\n    \"id\": \"JF.allocation.TendiesTradingCo.e61f512a-ed9c-4047-9ccf-224a5864158d\",\n    \"clientListID\": \"Hey! Welcome to DriveWealth Developer Docs!\",\n    \"status\": \"NEW\",\n    \"allocationsRequested\": 500,\n    \"allocationsCompleted\": 25,\n    \"unallocatedNotional\": 5320,\n    \"unallocatedQuantity\": 302,\n    \"comment\": \"All allocated and accounted for. 1::1::0 client note[empty], . timeMs=667 ratePerSec=1.50 msPerItem=667.00\",\n    \"createdWhen\": \"2022-12-22T16:04:46.724Z\"\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "25c3c892-9082-4b89-9d0c-55f0b04bac00",
          "name": "Advisor Reports",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "269466ff-eebd-4ed1-a710-d98dc890aa81",
              "name": "List Orders by Advisor",
              "request": {
                "name": "List Orders by Advisor",
                "description": {
                  "content": "Fetches a User's sub account orders allocations summary by date.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "users",
                    ":userID",
                    "managed",
                    "orders",
                    "summary"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "The specific request date in format YYYY-MM-DD.",
                        "type": "text/plain"
                      },
                      "key": "date",
                      "value": "<string>"
                    }
                  ],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The User's unique identifier.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "userID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "517754e6-417c-4b1a-a62c-d92a69fbe6be",
                  "name": "Fetching A User's Sub Account Orders Allocations Summary By Date was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "users",
                        ":userID",
                        "managed",
                        "orders",
                        "summary"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "date",
                          "value": "2022-12-25"
                        }
                      ],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) The User's unique identifier.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "userID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"id\": \"JF.allocation.TendiesTradingCo.e61f512a-ed9c-4047-9ccf-224a5864158d\",\n  \"accountNo\": \"DWBG000052\",\n  \"date\": \"2022-12-25\",\n  \"orders\": [\n    {\n      \"id\": \"IC.0e352bb7-9869-4233-9861-9673544efedd\",\n      \"orderNo\": \"ICDU023727\",\n      \"type\": \"MARKET\",\n      \"status\": \"FILLED\",\n      \"created\": \"2022-12-11T22:28:21.810Z\",\n      \"instrument\": {\n        \"id\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n        \"symbol\": \"MS\"\n      },\n      \"side\": \"B\",\n      \"averagePrice\": 1038.81,\n      \"orderQuantity\": 0.7219,\n      \"cumulativeQuantity\": 0.7219,\n      \"allocatedQuantity\": 0.7219,\n      \"unallocatedQuantity\": 302,\n      \"unallocatedNotional\": 5320,\n      \"allocations\": [\n        {\n          \"id\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"url\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"created\": \"2022-12-22T16:04:46.724Z\",\n          \"status\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"allocationsRequested\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"allocationsCompleted\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"unallocatedQuantity\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"unallocatedNotional\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"comment\": \"All allocated and accounted for. 1::1::0 client note[empty], . timeMs=667 ratePerSec=1.50 msPerItem=667.00\"\n        },\n        {\n          \"id\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"url\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"created\": \"2022-12-22T16:04:46.724Z\",\n          \"status\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"allocationsRequested\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"allocationsCompleted\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"unallocatedQuantity\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"unallocatedNotional\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"comment\": \"All allocated and accounted for. 1::1::0 client note[empty], . timeMs=667 ratePerSec=1.50 msPerItem=667.00\"\n        }\n      ]\n    },\n    {\n      \"id\": \"IC.0e352bb7-9869-4233-9861-9673544efedd\",\n      \"orderNo\": \"ICDU023727\",\n      \"type\": \"MARKET\",\n      \"status\": \"FILLED\",\n      \"created\": \"2022-12-11T22:28:21.810Z\",\n      \"instrument\": {\n        \"id\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n        \"symbol\": \"MS\"\n      },\n      \"side\": \"B\",\n      \"averagePrice\": 1038.81,\n      \"orderQuantity\": 0.7219,\n      \"cumulativeQuantity\": 0.7219,\n      \"allocatedQuantity\": 0.7219,\n      \"unallocatedQuantity\": 302,\n      \"unallocatedNotional\": 5320,\n      \"allocations\": [\n        {\n          \"id\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"url\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"created\": \"2022-12-22T16:04:46.724Z\",\n          \"status\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"allocationsRequested\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"allocationsCompleted\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"unallocatedQuantity\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"unallocatedNotional\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"comment\": \"All allocated and accounted for. 1::1::0 client note[empty], . timeMs=667 ratePerSec=1.50 msPerItem=667.00\"\n        },\n        {\n          \"id\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"url\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"created\": \"2022-12-22T16:04:46.724Z\",\n          \"status\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"allocationsRequested\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"allocationsCompleted\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"unallocatedQuantity\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"unallocatedNotional\": {\n            \"value\": \"<Error: Too many levels of nesting to fake this schema>\"\n          },\n          \"comment\": \"All allocated and accounted for. 1::1::0 client note[empty], . timeMs=667 ratePerSec=1.50 msPerItem=667.00\"\n        }\n      ]\n    }\n  ]\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "7f770bdf-adcf-49b6-8054-a1d92062e33a",
              "name": "List Allocations by Advisor",
              "request": {
                "name": "List Allocations by Advisor",
                "description": {
                  "content": "Fetches a user's sub account orders allocations by userID",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "users",
                    ":userID",
                    "managed",
                    "orders"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The date and time in which to start from.",
                        "type": "text/plain"
                      },
                      "key": "from",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The date and time in which to end at.",
                        "type": "text/plain"
                      },
                      "key": "to",
                      "value": "<string>"
                    }
                  ],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The User's unique identifier.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "userID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "16d85036-67b4-49d2-819c-da9ba1ec8b7b",
                  "name": "Fetching A user's Sub Account Orders Allocations By userID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "users",
                        ":userID",
                        "managed",
                        "orders"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "from",
                          "value": "2022-12-08T18:36:40.609Z"
                        },
                        {
                          "key": "to",
                          "value": "2022-12-25T18:36:40.609Z"
                        }
                      ],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) The User's unique identifier.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "userID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"riaID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n    \"orderID\": \"IC.0e352bb7-9869-4233-9861-9673544efedd\",\n    \"orderNo\": \"ICDU023727\",\n    \"orderType\": \"MARKET\",\n    \"createdWhen\": \"2022-12-11T22:28:21.810Z\",\n    \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n    \"symbol\": \"MS\",\n    \"side\": \"B\",\n    \"orderQty\": 0.7219,\n    \"cumQty\": 0.7219,\n    \"avgPx\": 1038.81,\n    \"allocations\": [\n      {\n        \"id\": \"JF.allocation.TendiesTradingCo.e61f512a-ed9c-4047-9ccf-224a5864158d\",\n        \"status\": \"NEW\",\n        \"unallocatedNotional\": 5320,\n        \"unallocatedQuantity\": 302\n      },\n      {\n        \"id\": \"JF.allocation.TendiesTradingCo.e61f512a-ed9c-4047-9ccf-224a5864158d\",\n        \"status\": \"NEW\",\n        \"unallocatedNotional\": 5320,\n        \"unallocatedQuantity\": 302\n      }\n    ]\n  },\n  {\n    \"riaID\": \"cc07f91b-7ee1-4868-b8fc-823c70a1b932\",\n    \"orderID\": \"IC.0e352bb7-9869-4233-9861-9673544efedd\",\n    \"orderNo\": \"ICDU023727\",\n    \"orderType\": \"MARKET\",\n    \"createdWhen\": \"2022-12-11T22:28:21.810Z\",\n    \"instrumentID\": \"3fb1e8a9-f7d5-4d90-95e2-43e7326b5636\",\n    \"symbol\": \"MS\",\n    \"side\": \"B\",\n    \"orderQty\": 0.7219,\n    \"cumQty\": 0.7219,\n    \"avgPx\": 1038.81,\n    \"allocations\": [\n      {\n        \"id\": \"JF.allocation.TendiesTradingCo.e61f512a-ed9c-4047-9ccf-224a5864158d\",\n        \"status\": \"NEW\",\n        \"unallocatedNotional\": 5320,\n        \"unallocatedQuantity\": 302\n      },\n      {\n        \"id\": \"JF.allocation.TendiesTradingCo.e61f512a-ed9c-4047-9ccf-224a5864158d\",\n        \"status\": \"NEW\",\n        \"unallocatedNotional\": 5320,\n        \"unallocatedQuantity\": 302\n      }\n    ]\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "15e973f9-2d39-4c9d-b410-72c0ff7a2594",
              "name": "Retrieve Beginning Of Day (BOD) by Advisor",
              "request": {
                "name": "Retrieve Beginning Of Day (BOD) by Advisor",
                "description": {
                  "content": "Fetches a list of sub accounts beginning of day holdings by userID",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "users",
                    ":userID",
                    "managed",
                    "bod"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The User's unique identifier.",
                        "type": "text/plain"
                      },
                      "type": "any",
                      "value": "<string>",
                      "key": "userID"
                    }
                  ]
                },
                "header": [
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "d4217ecc-b523-4445-976a-365dc0adffde",
                  "name": "Fetching A List Of Sub Accounts Beginning Of Day Holding By userID was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "users",
                        ":userID",
                        "managed",
                        "bod"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": [
                        {
                          "disabled": false,
                          "description": {
                            "content": "(Required) The User's unique identifier.",
                            "type": "text/plain"
                          },
                          "type": "any",
                          "value": "<string>",
                          "key": "userID"
                        }
                      ]
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"url\": \"'https://dtygu59lw0as9.cloudfront.net/_bod...\"\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "d59e37bc-87c1-475b-9817-49cc1bb13745",
          "name": "Funds",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [],
          "event": []
        },
        {
          "id": "49f3496f-b681-4f43-8585-b377d6887ce3",
          "name": "Portfolios",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [],
          "event": []
        },
        {
          "id": "e6f39da4-a580-4671-b34e-b14b428fa2bf",
          "name": "AutoPilot",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [],
          "event": []
        }
      ],
      "event": []
    },
    {
      "id": "90060496-5c8d-4dd7-9771-a4063563bce1",
      "name": "Market Data APIs",
      "item": [
        {
          "id": "1534f4fd-6106-43c6-a354-32ecf46fa0ab",
          "name": "Quotes",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "0b15c7c4-6add-41df-a6cd-9e92ae3b9260",
              "name": "Retrieve Quote (referential feed)",
              "request": {
                "name": "Retrieve Quote (referential feed)",
                "description": {
                  "content": "Fetch the realtime or 15 minute delayed Referential quote details for a specific security.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "quotes"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The ticker symbol of the associated instrument. Multiple ticker symbols separated by a comma may also be used.",
                        "type": "text/plain"
                      },
                      "key": "symbols",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "The quote details will be 15 minutes delayed.",
                        "type": "text/plain"
                      },
                      "key": "exchangeOverride",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The id of an instrument. Multiple instrumentIDs separated by a comma may also be used.",
                        "type": "text/plain"
                      },
                      "key": "instrumentIDs",
                      "value": "<string>"
                    },
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The unique identifier of the instrument. Multiple instrumentIDs separated by a comma may also be used.",
                        "type": "text/plain"
                      },
                      "key": "isins",
                      "value": "<string>"
                    }
                  ],
                  "variable": []
                },
                "header": [
                  {
                    "disabled": false,
                    "description": {
                      "content": "",
                      "type": "text/plain"
                    },
                    "key": "dw-customer-user-id",
                    "value": "<string>"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "0328ce55-3ad2-459d-a6c9-1d34e0f15314",
                  "name": "Fetch referential quote details was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "quotes"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "symbols",
                          "value": "MS"
                        },
                        {
                          "key": "exchangeOverride",
                          "value": "15MinDelayed"
                        },
                        {
                          "key": "instrumentIDs",
                          "value": "1179e8dd-2781-4ce9-842c-f05ded6a40d7"
                        },
                        {
                          "key": "isins",
                          "value": "US912810RC45"
                        }
                      ],
                      "variable": []
                    },
                    "header": [
                      {
                        "disabled": false,
                        "description": {
                          "content": "",
                          "type": "text/plain"
                        },
                        "key": "dw-customer-user-id",
                        "value": "66304da9-3h6f-2234-935f-ac6b7933d706"
                      },
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"symbol\": \"SBUX\",\n    \"bid\": 95.59,\n    \"ask\": 95.6,\n    \"lastTrade\": 95.6,\n    \"change\": 0.32,\n    \"open\": 95.65,\n    \"high\": 96.2,\n    \"low\": 95.23,\n    \"close\": 0,\n    \"priorClose\": 95.28,\n    \"volume\": 3973709,\n    \"marketCondition\": \"NORMAL\",\n    \"dataProvider\": \"NYSE\"\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            },
            {
              "id": "1c067bdf-aaf3-493e-bf77-03c04468d454",
              "name": "Retrieve Quote (consolidated feed)",
              "request": {
                "name": "Retrieve Quote (consolidated feed)",
                "description": {
                  "content": "Fetch the NBBO quote details for a specific security.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "quotes",
                    "vdr"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [
                    {
                      "disabled": false,
                      "description": {
                        "content": "(Required) The ticker symbol of the associated instrument.",
                        "type": "text/plain"
                      },
                      "key": "symbols",
                      "value": "<string>"
                    }
                  ],
                  "variable": []
                },
                "header": [
                  {
                    "disabled": false,
                    "description": {
                      "content": "",
                      "type": "text/plain"
                    },
                    "key": "dw-customer-user-id",
                    "value": "<string>"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "GET"
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "c1814ecd-c1e7-4c40-aa74-18d35089ad75",
                  "name": "Fetch NBBO quote details was Successful.",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "quotes",
                        "vdr"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [
                        {
                          "key": "symbols",
                          "value": "MS"
                        }
                      ],
                      "variable": []
                    },
                    "header": [
                      {
                        "disabled": false,
                        "description": {
                          "content": "",
                          "type": "text/plain"
                        },
                        "key": "dw-customer-user-id",
                        "value": "66304da9-3h6f-2234-935f-ac6b7933d706"
                      },
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "GET",
                    "body": {}
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "{\n  \"symbol\": \"MS\",\n  \"bid\": 86.12,\n  \"ask\": 85.14,\n  \"open\": 86.53,\n  \"high\": 86.85,\n  \"low\": 85.83,\n  \"timeOffset\": -35907805.69307475,\n  \"volume\": 2779731,\n  \"askSize\": 3,\n  \"bidSize\": 4,\n  \"change\": -1.33,\n  \"lastTradeExchange\": \"DX\",\n  \"bestBidExchange\": \"N\",\n  \"bestAskExchange\": \"Q\",\n  \"lastTrade\": 86.47,\n  \"lastTradeSize\": 2,\n  \"marketCondition\": \"NORMAL\",\n  \"tradeCount\": 29565,\n  \"close\": 0,\n  \"priorClose\": 86.86\n}",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        },
        {
          "id": "44af8ca9-42ea-479d-97a2-bdf7bed554ec",
          "name": "Charts",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [],
          "event": []
        },
        {
          "id": "13644a79-2e3f-466e-98b7-e588c7f1c5cb",
          "name": "Depth of Book",
          "description": {
            "content": "",
            "type": "text/plain"
          },
          "item": [
            {
              "id": "a3db60b9-685c-4754-92a1-9a0a914e0ffa",
              "name": "Retrieve Depth of Book",
              "request": {
                "name": "Retrieve Depth of Book",
                "description": {
                  "content": "Get the Depth of Book for an Instrument.\n\nFor now, this API only works with debt instruments, but will expand in the future.",
                  "type": "text/plain"
                },
                "url": {
                  "path": [
                    "quotes",
                    "depth"
                  ],
                  "host": [
                    "{{baseUrl}}"
                  ],
                  "query": [],
                  "variable": []
                },
                "header": [
                  {
                    "key": "Content-Type",
                    "value": "application/json"
                  },
                  {
                    "key": "Accept",
                    "value": "application/json"
                  },
                  {
                    "key": "dw-client-app-key",
                    "value": "{{dwAppKey}}"
                  }
                ],
                "method": "POST",
                "body": {
                  "mode": "raw",
                  "raw": "{\n  \"instrumentID\": \"<uuid>\",\n  \"quantity\": \"<double>\",\n  \"salesCredit\": {\n    \"currency\": \"<string>\",\n    \"amount\": \"<integer>\"\n  }\n}",
                  "options": {
                    "raw": {
                      "language": "json"
                    }
                  }
                }
              },
              "response": [
                {
                  "_": {
                    "postman_previewlanguage": "json"
                  },
                  "id": "9d7fc2ea-83d1-4256-928c-b12d9b7bb728",
                  "name": "Fetching Market data was successful",
                  "originalRequest": {
                    "url": {
                      "path": [
                        "quotes",
                        "depth"
                      ],
                      "host": [
                        "{{baseUrl}}"
                      ],
                      "query": [],
                      "variable": []
                    },
                    "header": [
                      {
                        "key": "Accept",
                        "value": "application/json"
                      },
                      {
                        "key": "dw-client-app-key",
                        "value": "{{dwAppKey}}"
                      }
                    ],
                    "method": "POST",
                    "body": {
                      "mode": "raw",
                      "raw": "{\n  \"instrumentID\": \"f6d3e213-4e6f-4ee3-8a9a-793027c62c57\",\n  \"quantity\": 3.14\n}",
                      "options": {
                        "raw": {
                          "language": "json"
                        }
                      }
                    }
                  },
                  "status": "OK",
                  "code": 200,
                  "header": [
                    {
                      "key": "Content-Type",
                      "value": "application/json"
                    }
                  ],
                  "body": "[\n  {\n    \"id\": \"f61b3240-6ab4-48bb-8f30-c160b7fba999\",\n    \"instrumentID\": \"206b06c2-6d46-4515-9340-678cb131f2cc\",\n    \"ISIN\": \"US105756BB58\",\n    \"CUSIP\": \"105756BB5\",\n    \"quantity\": 3,\n    \"salesCredit\": {\n      \"currency\": \"USD\",\n      \"amount\": 14\n    },\n    \"bidPrices\": [\n      {\n        \"bidPrice\": 98.882,\n        \"bidSize\": 100000,\n        \"bidYield\": 4.799,\n        \"minQty\": 150\n      },\n      {\n        \"bidPrice\": 98.872,\n        \"bidSize\": 230000,\n        \"bidYield\": 4.812,\n        \"minQty\": 112\n      }\n    ],\n    \"askPrices\": [\n      {\n        \"askPrice\": 98.884,\n        \"askSize\": 1000,\n        \"askYield\": 4.793,\n        \"minQty\": 150\n      },\n      {\n        \"askPrice\": 98.889,\n        \"askSize\": 250000,\n        \"askYield\": 4.768,\n        \"minQty\": 150\n      }\n    ],\n    \"effectiveBidPrices\": [\n      {\n        \"bidPrice\": 99.022,\n        \"bidSize\": 100000,\n        \"bidYield\": 4.739,\n        \"minQty\": 112\n      },\n      {\n        \"bidPrice\": 99.012,\n        \"bidSize\": 230000,\n        \"bidYield\": 4.812,\n        \"minQty\": 112\n      }\n    ],\n    \"effectiveAskPrices\": [\n      {\n        \"askPrice\": 98.744,\n        \"askSize\": 1000,\n        \"askYield\": 4.793,\n        \"minQty\": 150\n      },\n      {\n        \"askPrice\": 98.749,\n        \"askSize\": 250000,\n        \"askYield\": 4.768,\n        \"minQty\": 150\n      }\n    ],\n    \"recentTrades\": [\n      {\n        \"price\": 98.992,\n        \"quantity\": 10000,\n        \"yield\": 4.799,\n        \"side\": \"buy\",\n        \"date\": \"2017-07-21T17:32:28Z\"\n      }\n    ]\n  }\n]",
                  "cookie": []
                }
              ],
              "event": [],
              "protocolProfileBehavior": {
                "disableBodyPruning": true
              }
            }
          ],
          "event": []
        }
      ],
      "event": []
    }
  ],
  "event": [
    {
      "listen": "prerequest",
      "script": {
        "id": "db8d1d5b-e8fe-4493-a1e6-8d1251a5d648",
        "type": "text/javascript",
        "exec": [
          "var token = pm.environment.get(\"dwToken\");\nvar tokenExpiry = pm.environment.get(\"dwTokenExpiry\");\nvar clientID = pm.environment.get(\"dwClientID\");\nvar clientSecret = pm.environment.get(\"dwClientSecret\");\nvar appKey = pm.environment.get(\"dwAppKey\");\n\nif (\n\t(!token || new Date() > new Date(Number(tokenExpiry)))\n\t&& !pm.request.url.toString().includes(\"/auth/tokens\")\n\t&& clientID && clientSecret && appKey\n) {\n\tpm.sendRequest({\n\t\turl: pm.collectionVariables.get(\"baseUrl\") + \"/auth/tokens\",\n\t\tmethod: \"POST\",\n\t\theader: {\n\t\t\t\"Content-Type\": \"application/json\",\n\t\t\t\"Accept\": \"application/json\",\n\t\t\t\"dw-client-app-key\": appKey,\n\t\t},\n\t\tbody: {\n\t\t\tmode: \"raw\",\n\t\t\traw: JSON.stringify({\n\t\t\t\t\"clientID\": clientID,\n\t\t\t\t\"clientSecret\": clientSecret,\n\t\t\t})\n\t\t}\n\t}, function (err, res) {\n\t\tif (err === null && res.code === 200) {\n\t\t\tvar response = res.json();\n\t\t\tpm.environment.set(\"dwToken\", response.access_token);\n\t\t\tpm.environment.set(\"dwTokenExpiry\", Date.now() + response.expires_in * 1000)\n\t\t}\n\t});\n}\n\t\t\t"
        ]
      }
    }
  ],
  "variable": [
    {
      "type": "string",
      "value": "https://bo-api.drivewealth.io/back-office",
      "key": "baseUrl"
    }
  ],
  "auth": {
    "type": "bearer",
    "bearer": [
      {
        "type": "any",
        "value": "{{dwToken}}",
        "key": "token"
      }
    ]
  },
  "info": {
    "_postman_id": "8d1185ea-d3ac-490b-b848-37972e5be0d6",
    "name": "DriveWealth API",
    "schema": "https://schema.getpostman.com/json/collection/v2.1.0/collection.json",
    "description": {
      "content": "Welcome to the DriveWealth API Postman Collection!\n\nThese APIs match what you'll find browsing our [API Reference](https://developer.drivewealth.com/apis/reference/introduction).\n\nYou'll need the following environment variables:\n\n|Variable|Description|\n|-|-|\n|dwClientID|The client ID for your authentication.|\n|dwClientSecret|The secret for your authentication.|\n|dwAppKey|The app key unique to your integration.|\n\nThis collection will automatically attempt to refresh your token prior to an API request if it notices you do not have one set or the previously stored one has expired. If this is unsuccessful, an Authentication API is still bundled with the collection that you can invoke manually.\n\nVisit our [Developer Site](https://developer.drivewealth.com) to find more helpful resources and guides.",
      "type": "text/plain"
    }
  }
}