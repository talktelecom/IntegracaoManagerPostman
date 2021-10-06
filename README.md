# Integração Atendimento - Api Rest
Collection Postman - Integração Manager



## Token de acesso
```javascript

curl --location --request POST 'http://integracao.epbx.com.br/Service/oauth2/Token' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: OAuthEpbxManagerLocalCookie=gF-OrniEfLf3GuyEGz-xq4lq6xPh-_pMwDl0yJotEZWLSkp140m15URWnFXOp3XN430bBSX5yfBIqOl4A2mbIjGT7hdj_vcFWxFjXXD4DSssjLLIGB6uom-LPtVdQM0ZLxX1TSIe1GLd1O6zD2TVznQwRo2Ol0Y3huTOzJcg6MD6yyqHJuvRq38NxN0gOrhx1kUSxr_auUjcoVVI11quE32QFpGF9-_8uxk-CUoEzG_Eb7iJ1KYeGrvWeAli4jCynriqJiT7VqAzIu9_3tU-BRpfTN_Q-hMw4jZ81P1j4gTS7GJfayYYyqCM2XBpboN7xvsyi9nEFXWjHKWKXuci7SUrxaLh9bzPv1ycWYPOm0t4Yjq6FXBcf4buO7NKBIYAbecE-7RbIN7SWImvNFsYQ9pTkyCjVN_gR3w_Yvh6ZXc' \
--data-urlencode 'grant_type=password' \
--data-urlencode 'username=user' \
--data-urlencode 'password=pass' \
--data-urlencode 'client_id=abc'

```


## Logar ramal
```javascript
curl --location --request POST 'http://integracao.epbx.com.br/Service/Api/IntegracaoRamal/Logar' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer rt2MySuZa1k2xE4WyAJq6pZXcaekx2dCM9CfIgHgJeDCcQq27WcQcsc2oM5h0jlX9hripVDPKwwC9PWiU9ei9Sg2oeQFLbQlMdjg7TJcM3TBv99PDVLG54Is88M-PoE-TBQV_hRfw6KQ27w-vMp_o6Gbw7xK9avEK_ti6qysZmtLcrT3vkmtAcllrXg9zJq80gb_67syNbMwkhx7vb6oQz5fNPQBMIMOXG47h4qLSQKCG0DvvICK3FKh9dkx5s1KUCCdhefdOypr8elA_QZzrTR7_6UKhs_02bGsxDaBczZL_vFLCO9FO7Ffhp7e4LGGcmE36nmh4iElMP74Gk3_Ivw4wz6Cz3b0ZdGPS7PlCHxgWkUc1iR9vPy9CfXPAKE6R3n9SLxPs-DOikdKFZ_JAQ' \
--header 'Cookie: OAuthEpbxManagerLocalCookie=gF-OrniEfLf3GuyEGz-xq4lq6xPh-_pMwDl0yJotEZWLSkp140m15URWnFXOp3XN430bBSX5yfBIqOl4A2mbIjGT7hdj_vcFWxFjXXD4DSssjLLIGB6uom-LPtVdQM0ZLxX1TSIe1GLd1O6zD2TVznQwRo2Ol0Y3huTOzJcg6MD6yyqHJuvRq38NxN0gOrhx1kUSxr_auUjcoVVI11quE32QFpGF9-_8uxk-CUoEzG_Eb7iJ1KYeGrvWeAli4jCynriqJiT7VqAzIu9_3tU-BRpfTN_Q-hMw4jZ81P1j4gTS7GJfayYYyqCM2XBpboN7xvsyi9nEFXWjHKWKXuci7SUrxaLh9bzPv1ycWYPOm0t4Yjq6FXBcf4buO7NKBIYAbecE-7RbIN7SWImvNFsYQ9pTkyCjVN_gR3w_Yvh6ZXc' \
--data-raw '{
    "TipoLogon": "3",
    "ParametroLogon": "1010"
}'

```

## Deslogar ramal
```javascript
curl --location --request POST 'http://integracao.epbx.com.br/Service/Api/IntegracaoRamal/Deslogar' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer rt2MySuZa1k2xE4WyAJq6pZXcaekx2dCM9CfIgHgJeDCcQq27WcQcsc2oM5h0jlX9hripVDPKwwC9PWiU9ei9Sg2oeQFLbQlMdjg7TJcM3TBv99PDVLG54Is88M-PoE-TBQV_hRfw6KQ27w-vMp_o6Gbw7xK9avEK_ti6qysZmtLcrT3vkmtAcllrXg9zJq80gb_67syNbMwkhx7vb6oQz5fNPQBMIMOXG47h4qLSQKCG0DvvICK3FKh9dkx5s1KUCCdhefdOypr8elA_QZzrTR7_6UKhs_02bGsxDaBczZL_vFLCO9FO7Ffhp7e4LGGcmE36nmh4iElMP74Gk3_Ivw4wz6Cz3b0ZdGPS7PlCHxgWkUc1iR9vPy9CfXPAKE6R3n9SLxPs-DOikdKFZ_JAQ' \
--header 'Cookie: OAuthEpbxManagerLocalCookie=gF-OrniEfLf3GuyEGz-xq4lq6xPh-_pMwDl0yJotEZWLSkp140m15URWnFXOp3XN430bBSX5yfBIqOl4A2mbIjGT7hdj_vcFWxFjXXD4DSssjLLIGB6uom-LPtVdQM0ZLxX1TSIe1GLd1O6zD2TVznQwRo2Ol0Y3huTOzJcg6MD6yyqHJuvRq38NxN0gOrhx1kUSxr_auUjcoVVI11quE32QFpGF9-_8uxk-CUoEzG_Eb7iJ1KYeGrvWeAli4jCynriqJiT7VqAzIu9_3tU-BRpfTN_Q-hMw4jZ81P1j4gTS7GJfayYYyqCM2XBpboN7xvsyi9nEFXWjHKWKXuci7SUrxaLh9bzPv1ycWYPOm0t4Yjq6FXBcf4buO7NKBIYAbecE-7RbIN7SWImvNFsYQ9pTkyCjVN_gR3w_Yvh6ZXc' \
--data-raw ''
```



## Discar
```javascript
curl --location --request POST 'http://integracao.epbx.com.br/Service/Api/IntegracaoRamal/Discar' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer rt2MySuZa1k2xE4WyAJq6pZXcaekx2dCM9CfIgHgJeDCcQq27WcQcsc2oM5h0jlX9hripVDPKwwC9PWiU9ei9Sg2oeQFLbQlMdjg7TJcM3TBv99PDVLG54Is88M-PoE-TBQV_hRfw6KQ27w-vMp_o6Gbw7xK9avEK_ti6qysZmtLcrT3vkmtAcllrXg9zJq80gb_67syNbMwkhx7vb6oQz5fNPQBMIMOXG47h4qLSQKCG0DvvICK3FKh9dkx5s1KUCCdhefdOypr8elA_QZzrTR7_6UKhs_02bGsxDaBczZL_vFLCO9FO7Ffhp7e4LGGcmE36nmh4iElMP74Gk3_Ivw4wz6Cz3b0ZdGPS7PlCHxgWkUc1iR9vPy9CfXPAKE6R3n9SLxPs-DOikdKFZ_JAQ' \
--header 'Cookie: OAuthEpbxManagerLocalCookie=gF-OrniEfLf3GuyEGz-xq4lq6xPh-_pMwDl0yJotEZWLSkp140m15URWnFXOp3XN430bBSX5yfBIqOl4A2mbIjGT7hdj_vcFWxFjXXD4DSssjLLIGB6uom-LPtVdQM0ZLxX1TSIe1GLd1O6zD2TVznQwRo2Ol0Y3huTOzJcg6MD6yyqHJuvRq38NxN0gOrhx1kUSxr_auUjcoVVI11quE32QFpGF9-_8uxk-CUoEzG_Eb7iJ1KYeGrvWeAli4jCynriqJiT7VqAzIu9_3tU-BRpfTN_Q-hMw4jZ81P1j4gTS7GJfayYYyqCM2XBpboN7xvsyi9nEFXWjHKWKXuci7SUrxaLh9bzPv1ycWYPOm0t4Yjq6FXBcf4buO7NKBIYAbecE-7RbIN7SWImvNFsYQ9pTkyCjVN_gR3w_Yvh6ZXc' \
--data-raw '{
    "TipoDiscagem": "1",
    "Numero": "1123910000"
}'
```


## Desligar 
```javascript
curl --location --request POST 'http://integracao.epbx.com.br/Service/Api/IntegracaoRamal/DesligarChamada' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer rt2MySuZa1k2xE4WyAJq6pZXcaekx2dCM9CfIgHgJeDCcQq27WcQcsc2oM5h0jlX9hripVDPKwwC9PWiU9ei9Sg2oeQFLbQlMdjg7TJcM3TBv99PDVLG54Is88M-PoE-TBQV_hRfw6KQ27w-vMp_o6Gbw7xK9avEK_ti6qysZmtLcrT3vkmtAcllrXg9zJq80gb_67syNbMwkhx7vb6oQz5fNPQBMIMOXG47h4qLSQKCG0DvvICK3FKh9dkx5s1KUCCdhefdOypr8elA_QZzrTR7_6UKhs_02bGsxDaBczZL_vFLCO9FO7Ffhp7e4LGGcmE36nmh4iElMP74Gk3_Ivw4wz6Cz3b0ZdGPS7PlCHxgWkUc1iR9vPy9CfXPAKE6R3n9SLxPs-DOikdKFZ_JAQ' \
--header 'Cookie: OAuthEpbxManagerLocalCookie=gF-OrniEfLf3GuyEGz-xq4lq6xPh-_pMwDl0yJotEZWLSkp140m15URWnFXOp3XN430bBSX5yfBIqOl4A2mbIjGT7hdj_vcFWxFjXXD4DSssjLLIGB6uom-LPtVdQM0ZLxX1TSIe1GLd1O6zD2TVznQwRo2Ol0Y3huTOzJcg6MD6yyqHJuvRq38NxN0gOrhx1kUSxr_auUjcoVVI11quE32QFpGF9-_8uxk-CUoEzG_Eb7iJ1KYeGrvWeAli4jCynriqJiT7VqAzIu9_3tU-BRpfTN_Q-hMw4jZ81P1j4gTS7GJfayYYyqCM2XBpboN7xvsyi9nEFXWjHKWKXuci7SUrxaLh9bzPv1ycWYPOm0t4Yjq6FXBcf4buO7NKBIYAbecE-7RbIN7SWImvNFsYQ9pTkyCjVN_gR3w_Yvh6ZXc' \
--data-raw ''
```


## Listar intervalos
```javascript
curl --location --request GET 'http://integracao.epbx.com.br/Service/Api/IntegracaoRamal/Intervalos' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer rt2MySuZa1k2xE4WyAJq6pZXcaekx2dCM9CfIgHgJeDCcQq27WcQcsc2oM5h0jlX9hripVDPKwwC9PWiU9ei9Sg2oeQFLbQlMdjg7TJcM3TBv99PDVLG54Is88M-PoE-TBQV_hRfw6KQ27w-vMp_o6Gbw7xK9avEK_ti6qysZmtLcrT3vkmtAcllrXg9zJq80gb_67syNbMwkhx7vb6oQz5fNPQBMIMOXG47h4qLSQKCG0DvvICK3FKh9dkx5s1KUCCdhefdOypr8elA_QZzrTR7_6UKhs_02bGsxDaBczZL_vFLCO9FO7Ffhp7e4LGGcmE36nmh4iElMP74Gk3_Ivw4wz6Cz3b0ZdGPS7PlCHxgWkUc1iR9vPy9CfXPAKE6R3n9SLxPs-DOikdKFZ_JAQ' \
--header 'Cookie: OAuthEpbxManagerLocalCookie=gF-OrniEfLf3GuyEGz-xq4lq6xPh-_pMwDl0yJotEZWLSkp140m15URWnFXOp3XN430bBSX5yfBIqOl4A2mbIjGT7hdj_vcFWxFjXXD4DSssjLLIGB6uom-LPtVdQM0ZLxX1TSIe1GLd1O6zD2TVznQwRo2Ol0Y3huTOzJcg6MD6yyqHJuvRq38NxN0gOrhx1kUSxr_auUjcoVVI11quE32QFpGF9-_8uxk-CUoEzG_Eb7iJ1KYeGrvWeAli4jCynriqJiT7VqAzIu9_3tU-BRpfTN_Q-hMw4jZ81P1j4gTS7GJfayYYyqCM2XBpboN7xvsyi9nEFXWjHKWKXuci7SUrxaLh9bzPv1ycWYPOm0t4Yjq6FXBcf4buO7NKBIYAbecE-7RbIN7SWImvNFsYQ9pTkyCjVN_gR3w_Yvh6ZXc' \
--data-raw ''
```

## Alterar intervalo
```javascript
curl --location --request POST 'http://integracao.epbx.com.br/Service/Api/IntegracaoRamal/AlterarIntervalo' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer rt2MySuZa1k2xE4WyAJq6pZXcaekx2dCM9CfIgHgJeDCcQq27WcQcsc2oM5h0jlX9hripVDPKwwC9PWiU9ei9Sg2oeQFLbQlMdjg7TJcM3TBv99PDVLG54Is88M-PoE-TBQV_hRfw6KQ27w-vMp_o6Gbw7xK9avEK_ti6qysZmtLcrT3vkmtAcllrXg9zJq80gb_67syNbMwkhx7vb6oQz5fNPQBMIMOXG47h4qLSQKCG0DvvICK3FKh9dkx5s1KUCCdhefdOypr8elA_QZzrTR7_6UKhs_02bGsxDaBczZL_vFLCO9FO7Ffhp7e4LGGcmE36nmh4iElMP74Gk3_Ivw4wz6Cz3b0ZdGPS7PlCHxgWkUc1iR9vPy9CfXPAKE6R3n9SLxPs-DOikdKFZ_JAQ' \
--header 'Cookie: OAuthEpbxManagerLocalCookie=gF-OrniEfLf3GuyEGz-xq4lq6xPh-_pMwDl0yJotEZWLSkp140m15URWnFXOp3XN430bBSX5yfBIqOl4A2mbIjGT7hdj_vcFWxFjXXD4DSssjLLIGB6uom-LPtVdQM0ZLxX1TSIe1GLd1O6zD2TVznQwRo2Ol0Y3huTOzJcg6MD6yyqHJuvRq38NxN0gOrhx1kUSxr_auUjcoVVI11quE32QFpGF9-_8uxk-CUoEzG_Eb7iJ1KYeGrvWeAli4jCynriqJiT7VqAzIu9_3tU-BRpfTN_Q-hMw4jZ81P1j4gTS7GJfayYYyqCM2XBpboN7xvsyi9nEFXWjHKWKXuci7SUrxaLh9bzPv1ycWYPOm0t4Yjq6FXBcf4buO7NKBIYAbecE-7RbIN7SWImvNFsYQ9pTkyCjVN_gR3w_Yvh6ZXc' \
--data-raw '{
    "Codigo": "3"
}'
```

## Listar intervalo Atual do Ramal
```javascript
curl --location --request GET 'http://integracao.epbx.com.br/Service/Api/IntegracaoRamal/IntervaloAtual' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer rt2MySuZa1k2xE4WyAJq6pZXcaekx2dCM9CfIgHgJeDCcQq27WcQcsc2oM5h0jlX9hripVDPKwwC9PWiU9ei9Sg2oeQFLbQlMdjg7TJcM3TBv99PDVLG54Is88M-PoE-TBQV_hRfw6KQ27w-vMp_o6Gbw7xK9avEK_ti6qysZmtLcrT3vkmtAcllrXg9zJq80gb_67syNbMwkhx7vb6oQz5fNPQBMIMOXG47h4qLSQKCG0DvvICK3FKh9dkx5s1KUCCdhefdOypr8elA_QZzrTR7_6UKhs_02bGsxDaBczZL_vFLCO9FO7Ffhp7e4LGGcmE36nmh4iElMP74Gk3_Ivw4wz6Cz3b0ZdGPS7PlCHxgWkUc1iR9vPy9CfXPAKE6R3n9SLxPs-DOikdKFZ_JAQ' \
--header 'Cookie: OAuthEpbxManagerLocalCookie=gF-OrniEfLf3GuyEGz-xq4lq6xPh-_pMwDl0yJotEZWLSkp140m15URWnFXOp3XN430bBSX5yfBIqOl4A2mbIjGT7hdj_vcFWxFjXXD4DSssjLLIGB6uom-LPtVdQM0ZLxX1TSIe1GLd1O6zD2TVznQwRo2Ol0Y3huTOzJcg6MD6yyqHJuvRq38NxN0gOrhx1kUSxr_auUjcoVVI11quE32QFpGF9-_8uxk-CUoEzG_Eb7iJ1KYeGrvWeAli4jCynriqJiT7VqAzIu9_3tU-BRpfTN_Q-hMw4jZ81P1j4gTS7GJfayYYyqCM2XBpboN7xvsyi9nEFXWjHKWKXuci7SUrxaLh9bzPv1ycWYPOm0t4Yjq6FXBcf4buO7NKBIYAbecE-7RbIN7SWImvNFsYQ9pTkyCjVN_gR3w_Yvh6ZXc' \
--data-raw ''
```

## Listar informaçãoes da chamada em curso 
```javascript
curl --location --request GET 'http://integracao.epbx.com.br/Service/Api/IntegracaoRamal/ChamadaAtiva' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer rt2MySuZa1k2xE4WyAJq6pZXcaekx2dCM9CfIgHgJeDCcQq27WcQcsc2oM5h0jlX9hripVDPKwwC9PWiU9ei9Sg2oeQFLbQlMdjg7TJcM3TBv99PDVLG54Is88M-PoE-TBQV_hRfw6KQ27w-vMp_o6Gbw7xK9avEK_ti6qysZmtLcrT3vkmtAcllrXg9zJq80gb_67syNbMwkhx7vb6oQz5fNPQBMIMOXG47h4qLSQKCG0DvvICK3FKh9dkx5s1KUCCdhefdOypr8elA_QZzrTR7_6UKhs_02bGsxDaBczZL_vFLCO9FO7Ffhp7e4LGGcmE36nmh4iElMP74Gk3_Ivw4wz6Cz3b0ZdGPS7PlCHxgWkUc1iR9vPy9CfXPAKE6R3n9SLxPs-DOikdKFZ_JAQ' \
--header 'Cookie: OAuthEpbxManagerLocalCookie=gF-OrniEfLf3GuyEGz-xq4lq6xPh-_pMwDl0yJotEZWLSkp140m15URWnFXOp3XN430bBSX5yfBIqOl4A2mbIjGT7hdj_vcFWxFjXXD4DSssjLLIGB6uom-LPtVdQM0ZLxX1TSIe1GLd1O6zD2TVznQwRo2Ol0Y3huTOzJcg6MD6yyqHJuvRq38NxN0gOrhx1kUSxr_auUjcoVVI11quE32QFpGF9-_8uxk-CUoEzG_Eb7iJ1KYeGrvWeAli4jCynriqJiT7VqAzIu9_3tU-BRpfTN_Q-hMw4jZ81P1j4gTS7GJfayYYyqCM2XBpboN7xvsyi9nEFXWjHKWKXuci7SUrxaLh9bzPv1ycWYPOm0t4Yjq6FXBcf4buO7NKBIYAbecE-7RbIN7SWImvNFsYQ9pTkyCjVN_gR3w_Yvh6ZXc' \
--data-raw ''
```
 

## Importar Mailing Lote
```javascript
curl --location --request POST 'http://integracao.epbx.com.br/Service/Api/CampanhaDiscagem/Lote?campanhaId=38' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer vAcyElQYZdRo0CSmb8ksNbo4YNI939h7B8JrS-QvtI51fARvNNspRrqfWhIJ87FBz3c2LvJcjnnehKcNs7QT2shUabIUqlCrC-ltejuAguC3fOerO5KYyhR6SIdw8sza95BE4YXNeiZ2sRitMnDIH_0cnP7-kfXSpVAo5KkxOfQ2BIBmsqYV8HBZ4-uHVKMvmm7pnj249bc__QDVtfkyfIcawGip0tI7xOE534nFZg5MrXVL-Y-VXIVfmR6hw1ggBzxnXZOLbaVh2_wrIjPWLMpxyUfIG9u5PnarFP2A0JD9SBizacx_5IOCXHq2Q7F6tpXKDhJD79sqvoDm20APkuImcpvLtKetSxpA7fluRmMJiHSv_AmVT5oHVDLMeNIQgBxxnPi15V08xpGafcGTSq4LaTp1wOKoP1MbEbv8t4I' \
--header 'Cookie: OAuthEpbxManagerLocalCookie=UPWp8mh2B2OZa1D46tz5C-s_ymuUvGM28eOj-BLqnrOE-OcS-LYI5NpkN0ZTMo31GmL5jcqnrBs2A14Ap1dmUtAHbVqAMzkBEquCT6DqqslZTyspkryGxtf1xD5lz6mGX7ZZ3RgJ4bMUTFLibFhGdEgnlgyJdz1GXEHw4m7EJRLYjYnfx42ofdlrmycbLqKdaWkTdMKdSxhSKgDcDy71501DqTq_pHzPD6sx8t8QgdqwzHJ0e36bhPfZ-CyT22-yF9_9hjtpizNY71ZMAxQ7wAszsvaLv01XrFInzCgVX1lGeSVvB5bM7zAASc1T74hrbKDEbAre3Hn_AnXFcrYa2xs0zCpgnVZuPMPRbcldM1__6J5DD9R6XofmbcexZOs3lK6l8dYd4MjzBkAX9KbmlYmwm9uiNtwoT6XDnfiAikA' \
--data-raw '[
  {
    "CodigoCliente": "213456",
    "Nome": "Talk Telecom",
    "DDD": "11",
    "Numero": "23910000",
    "Detalhe": "Info1,Info2,Info3"
  }
]'
```
 
## Agendamento
```javascript
curl --location --request POST 'http://integracao.epbx.com.br/Service/Api/Atendimento/Agendamento' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer vAcyElQYZdRo0CSmb8ksNbo4YNI939h7B8JrS-QvtI51fARvNNspRrqfWhIJ87FBz3c2LvJcjnnehKcNs7QT2shUabIUqlCrC-ltejuAguC3fOerO5KYyhR6SIdw8sza95BE4YXNeiZ2sRitMnDIH_0cnP7-kfXSpVAo5KkxOfQ2BIBmsqYV8HBZ4-uHVKMvmm7pnj249bc__QDVtfkyfIcawGip0tI7xOE534nFZg5MrXVL-Y-VXIVfmR6hw1ggBzxnXZOLbaVh2_wrIjPWLMpxyUfIG9u5PnarFP2A0JD9SBizacx_5IOCXHq2Q7F6tpXKDhJD79sqvoDm20APkuImcpvLtKetSxpA7fluRmMJiHSv_AmVT5oHVDLMeNIQgBxxnPi15V08xpGafcGTSq4LaTp1wOKoP1MbEbv8t4I' \
--header 'Cookie: OAuthEpbxManagerLocalCookie=UPWp8mh2B2OZa1D46tz5C-s_ymuUvGM28eOj-BLqnrOE-OcS-LYI5NpkN0ZTMo31GmL5jcqnrBs2A14Ap1dmUtAHbVqAMzkBEquCT6DqqslZTyspkryGxtf1xD5lz6mGX7ZZ3RgJ4bMUTFLibFhGdEgnlgyJdz1GXEHw4m7EJRLYjYnfx42ofdlrmycbLqKdaWkTdMKdSxhSKgDcDy71501DqTq_pHzPD6sx8t8QgdqwzHJ0e36bhPfZ-CyT22-yF9_9hjtpizNY71ZMAxQ7wAszsvaLv01XrFInzCgVX1lGeSVvB5bM7zAASc1T74hrbKDEbAre3Hn_AnXFcrYa2xs0zCpgnVZuPMPRbcldM1__6J5DD9R6XofmbcexZOs3lK6l8dYd4MjzBkAX9KbmlYmwm9uiNtwoT6XDnfiAikA' \
--data-raw '{
    "Campanha": "578",
    "CodCliente": "123456",
    "DDD": "11",
    "Telefone": "997422080",
    "DataHora": "2018-04-03T13:35:00",
    "Ramal": 1009,
    "NomeCliente": "Wagner"
}'
```

## Contato Negativo
```javascript
curl --location --request POST 'http://integracao.epbx.com.br/Service/Api/Atendimento/ContatoNegativo' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer vAcyElQYZdRo0CSmb8ksNbo4YNI939h7B8JrS-QvtI51fARvNNspRrqfWhIJ87FBz3c2LvJcjnnehKcNs7QT2shUabIUqlCrC-ltejuAguC3fOerO5KYyhR6SIdw8sza95BE4YXNeiZ2sRitMnDIH_0cnP7-kfXSpVAo5KkxOfQ2BIBmsqYV8HBZ4-uHVKMvmm7pnj249bc__QDVtfkyfIcawGip0tI7xOE534nFZg5MrXVL-Y-VXIVfmR6hw1ggBzxnXZOLbaVh2_wrIjPWLMpxyUfIG9u5PnarFP2A0JD9SBizacx_5IOCXHq2Q7F6tpXKDhJD79sqvoDm20APkuImcpvLtKetSxpA7fluRmMJiHSv_AmVT5oHVDLMeNIQgBxxnPi15V08xpGafcGTSq4LaTp1wOKoP1MbEbv8t4I' \
--header 'Cookie: OAuthEpbxManagerLocalCookie=UPWp8mh2B2OZa1D46tz5C-s_ymuUvGM28eOj-BLqnrOE-OcS-LYI5NpkN0ZTMo31GmL5jcqnrBs2A14Ap1dmUtAHbVqAMzkBEquCT6DqqslZTyspkryGxtf1xD5lz6mGX7ZZ3RgJ4bMUTFLibFhGdEgnlgyJdz1GXEHw4m7EJRLYjYnfx42ofdlrmycbLqKdaWkTdMKdSxhSKgDcDy71501DqTq_pHzPD6sx8t8QgdqwzHJ0e36bhPfZ-CyT22-yF9_9hjtpizNY71ZMAxQ7wAszsvaLv01XrFInzCgVX1lGeSVvB5bM7zAASc1T74hrbKDEbAre3Hn_AnXFcrYa2xs0zCpgnVZuPMPRbcldM1__6J5DD9R6XofmbcexZOs3lK6l8dYd4MjzBkAX9KbmlYmwm9uiNtwoT6XDnfiAikA' \
--data-raw '{
    "Campanha": "3230",
    "CodCliente": "123456",
    "DDD": "11",
    "Telefone": "997422080",
    "Prioridade":""
}'
```


## Remove Cliente
```javascript
curl --location --request POST 'http://integracao.epbx.com.br/Service/Api/Atendimento/RemoveCliente' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer vAcyElQYZdRo0CSmb8ksNbo4YNI939h7B8JrS-QvtI51fARvNNspRrqfWhIJ87FBz3c2LvJcjnnehKcNs7QT2shUabIUqlCrC-ltejuAguC3fOerO5KYyhR6SIdw8sza95BE4YXNeiZ2sRitMnDIH_0cnP7-kfXSpVAo5KkxOfQ2BIBmsqYV8HBZ4-uHVKMvmm7pnj249bc__QDVtfkyfIcawGip0tI7xOE534nFZg5MrXVL-Y-VXIVfmR6hw1ggBzxnXZOLbaVh2_wrIjPWLMpxyUfIG9u5PnarFP2A0JD9SBizacx_5IOCXHq2Q7F6tpXKDhJD79sqvoDm20APkuImcpvLtKetSxpA7fluRmMJiHSv_AmVT5oHVDLMeNIQgBxxnPi15V08xpGafcGTSq4LaTp1wOKoP1MbEbv8t4I' \
--header 'Cookie: OAuthEpbxManagerLocalCookie=UPWp8mh2B2OZa1D46tz5C-s_ymuUvGM28eOj-BLqnrOE-OcS-LYI5NpkN0ZTMo31GmL5jcqnrBs2A14Ap1dmUtAHbVqAMzkBEquCT6DqqslZTyspkryGxtf1xD5lz6mGX7ZZ3RgJ4bMUTFLibFhGdEgnlgyJdz1GXEHw4m7EJRLYjYnfx42ofdlrmycbLqKdaWkTdMKdSxhSKgDcDy71501DqTq_pHzPD6sx8t8QgdqwzHJ0e36bhPfZ-CyT22-yF9_9hjtpizNY71ZMAxQ7wAszsvaLv01XrFInzCgVX1lGeSVvB5bM7zAASc1T74hrbKDEbAre3Hn_AnXFcrYa2xs0zCpgnVZuPMPRbcldM1__6J5DD9R6XofmbcexZOs3lK6l8dYd4MjzBkAX9KbmlYmwm9uiNtwoT6XDnfiAikA' \
--data-raw '{
    "Campanha": "168",
    "CodCliente": "1234",
    "Geral": "1"
}'
```

## Dupplicar Campanha
```javascript
curl --location --request POST 'http://integracao.epbx.com.br/Service/Api/Campanha/Duplicar?CampanhaId=704' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer vAcyElQYZdRo0CSmb8ksNbo4YNI939h7B8JrS-QvtI51fARvNNspRrqfWhIJ87FBz3c2LvJcjnnehKcNs7QT2shUabIUqlCrC-ltejuAguC3fOerO5KYyhR6SIdw8sza95BE4YXNeiZ2sRitMnDIH_0cnP7-kfXSpVAo5KkxOfQ2BIBmsqYV8HBZ4-uHVKMvmm7pnj249bc__QDVtfkyfIcawGip0tI7xOE534nFZg5MrXVL-Y-VXIVfmR6hw1ggBzxnXZOLbaVh2_wrIjPWLMpxyUfIG9u5PnarFP2A0JD9SBizacx_5IOCXHq2Q7F6tpXKDhJD79sqvoDm20APkuImcpvLtKetSxpA7fluRmMJiHSv_AmVT5oHVDLMeNIQgBxxnPi15V08xpGafcGTSq4LaTp1wOKoP1MbEbv8t4I' \
--header 'Cookie: OAuthEpbxManagerLocalCookie=UPWp8mh2B2OZa1D46tz5C-s_ymuUvGM28eOj-BLqnrOE-OcS-LYI5NpkN0ZTMo31GmL5jcqnrBs2A14Ap1dmUtAHbVqAMzkBEquCT6DqqslZTyspkryGxtf1xD5lz6mGX7ZZ3RgJ4bMUTFLibFhGdEgnlgyJdz1GXEHw4m7EJRLYjYnfx42ofdlrmycbLqKdaWkTdMKdSxhSKgDcDy71501DqTq_pHzPD6sx8t8QgdqwzHJ0e36bhPfZ-CyT22-yF9_9hjtpizNY71ZMAxQ7wAszsvaLv01XrFInzCgVX1lGeSVvB5bM7zAASc1T74hrbKDEbAre3Hn_AnXFcrYa2xs0zCpgnVZuPMPRbcldM1__6J5DD9R6XofmbcexZOs3lK6l8dYd4MjzBkAX9KbmlYmwm9uiNtwoT6XDnfiAikA' \
--data-raw '{
    "CodigoCliente": "213456",
    "Nome": "Talk Telecom",
    "DDD": "11",
    "Numero": "23910000",
    "Detalhe": "Info1,Info2,Info3"
}'
```


## LImpar Campanha
```javascript
curl --location --request POST 'http://integracao.epbx.com.br/Service/Api/Campanha/ZerarCampanha?CampanhaId=705' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer vAcyElQYZdRo0CSmb8ksNbo4YNI939h7B8JrS-QvtI51fARvNNspRrqfWhIJ87FBz3c2LvJcjnnehKcNs7QT2shUabIUqlCrC-ltejuAguC3fOerO5KYyhR6SIdw8sza95BE4YXNeiZ2sRitMnDIH_0cnP7-kfXSpVAo5KkxOfQ2BIBmsqYV8HBZ4-uHVKMvmm7pnj249bc__QDVtfkyfIcawGip0tI7xOE534nFZg5MrXVL-Y-VXIVfmR6hw1ggBzxnXZOLbaVh2_wrIjPWLMpxyUfIG9u5PnarFP2A0JD9SBizacx_5IOCXHq2Q7F6tpXKDhJD79sqvoDm20APkuImcpvLtKetSxpA7fluRmMJiHSv_AmVT5oHVDLMeNIQgBxxnPi15V08xpGafcGTSq4LaTp1wOKoP1MbEbv8t4I' \
--header 'Cookie: OAuthEpbxManagerLocalCookie=UPWp8mh2B2OZa1D46tz5C-s_ymuUvGM28eOj-BLqnrOE-OcS-LYI5NpkN0ZTMo31GmL5jcqnrBs2A14Ap1dmUtAHbVqAMzkBEquCT6DqqslZTyspkryGxtf1xD5lz6mGX7ZZ3RgJ4bMUTFLibFhGdEgnlgyJdz1GXEHw4m7EJRLYjYnfx42ofdlrmycbLqKdaWkTdMKdSxhSKgDcDy71501DqTq_pHzPD6sx8t8QgdqwzHJ0e36bhPfZ-CyT22-yF9_9hjtpizNY71ZMAxQ7wAszsvaLv01XrFInzCgVX1lGeSVvB5bM7zAASc1T74hrbKDEbAre3Hn_AnXFcrYa2xs0zCpgnVZuPMPRbcldM1__6J5DD9R6XofmbcexZOs3lK6l8dYd4MjzBkAX9KbmlYmwm9uiNtwoT6XDnfiAikA' \
--data-raw '{"CampanhaId":705,"MantemAgendamento":false}'
```



