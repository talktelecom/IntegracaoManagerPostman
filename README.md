# Integração Atendimento - Api Rest
Collection Postman - Integração Manager



## Autenticar 
```javascript

curl --location --request POST 'http://integracao.epbx.com.br/Service/oauth2/Token' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: OAuthEpbxManagerLocalCookie=gF-OrniEfLf3GuyEGz-xq4lq6xPh-_pMwDl0yJotEZWLSkp140m15URWnFXOp3XN430bBSX5yfBIqOl4A2mbIjGT7hdj_vcFWxFjXXD4DSssjLLIGB6uom-LPtVdQM0ZLxX1TSIe1GLd1O6zD2TVznQwRo2Ol0Y3huTOzJcg6MD6yyqHJuvRq38NxN0gOrhx1kUSxr_auUjcoVVI11quE32QFpGF9-_8uxk-CUoEzG_Eb7iJ1KYeGrvWeAli4jCynriqJiT7VqAzIu9_3tU-BRpfTN_Q-hMw4jZ81P1j4gTS7GJfayYYyqCM2XBpboN7xvsyi9nEFXWjHKWKXuci7SUrxaLh9bzPv1ycWYPOm0t4Yjq6FXBcf4buO7NKBIYAbecE-7RbIN7SWImvNFsYQ9pTkyCjVN_gR3w_Yvh6ZXc' \
--data-urlencode 'grant_type=password' \
--data-urlencode 'username=dev' \
--data-urlencode 'password=1234' \
--data-urlencode 'client_id=abc'

```



## Logar Ramal
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

## Deslogar Ramal
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
    "Numero": "11997422080"
}'
```


## Listar Intervalos
```javascript
curl --location --request GET 'http://integracao.epbx.com.br/Service/Api/IntegracaoRamal/Intervalos' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer rt2MySuZa1k2xE4WyAJq6pZXcaekx2dCM9CfIgHgJeDCcQq27WcQcsc2oM5h0jlX9hripVDPKwwC9PWiU9ei9Sg2oeQFLbQlMdjg7TJcM3TBv99PDVLG54Is88M-PoE-TBQV_hRfw6KQ27w-vMp_o6Gbw7xK9avEK_ti6qysZmtLcrT3vkmtAcllrXg9zJq80gb_67syNbMwkhx7vb6oQz5fNPQBMIMOXG47h4qLSQKCG0DvvICK3FKh9dkx5s1KUCCdhefdOypr8elA_QZzrTR7_6UKhs_02bGsxDaBczZL_vFLCO9FO7Ffhp7e4LGGcmE36nmh4iElMP74Gk3_Ivw4wz6Cz3b0ZdGPS7PlCHxgWkUc1iR9vPy9CfXPAKE6R3n9SLxPs-DOikdKFZ_JAQ' \
--header 'Cookie: OAuthEpbxManagerLocalCookie=gF-OrniEfLf3GuyEGz-xq4lq6xPh-_pMwDl0yJotEZWLSkp140m15URWnFXOp3XN430bBSX5yfBIqOl4A2mbIjGT7hdj_vcFWxFjXXD4DSssjLLIGB6uom-LPtVdQM0ZLxX1TSIe1GLd1O6zD2TVznQwRo2Ol0Y3huTOzJcg6MD6yyqHJuvRq38NxN0gOrhx1kUSxr_auUjcoVVI11quE32QFpGF9-_8uxk-CUoEzG_Eb7iJ1KYeGrvWeAli4jCynriqJiT7VqAzIu9_3tU-BRpfTN_Q-hMw4jZ81P1j4gTS7GJfayYYyqCM2XBpboN7xvsyi9nEFXWjHKWKXuci7SUrxaLh9bzPv1ycWYPOm0t4Yjq6FXBcf4buO7NKBIYAbecE-7RbIN7SWImvNFsYQ9pTkyCjVN_gR3w_Yvh6ZXc' \
--data-raw ''
```



