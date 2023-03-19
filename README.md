# Windows 11 ative sem uma chave
Uma forma de ativar qualquer versão do Windows 11 usando o servidor de chaves do MsGuides.
## Ative o  Windows 11 usando uma chave cliente KMS gratuita
## Ativação Manual

Execute o aplicativo Prompt de Comando como administrador.
Clique no botão Iniciar, procure por “cmd” e [execute-o com direitos de administrador](https://msguides.com/open-command-prompt-admin).

## Instale a chave do cliente KMS
```
Use o comando “slmgr /ipk kmsclientkey” para instalar uma chave de licença (kmsclientkey é a chave de ativação que corresponde à sua edição do Windows).

Exemplo: 
slmgr /ipk NPPR9-FWDCX-D2C8J-H872K-2YT43

A seguir está a lista de chaves de licença do Windows 11 Volume.

Home: TX9XD-98N7V-6WMQ6-BX7FG-H8Q99
Home N: 3KHY7-WNT83-DGQKR-F7HPR-844BM
Home Single Language: 7HNRX-D7KGG-3K4RQ-4WPJ4-YTDFH
Home Country Specific: PVMJN-6DFY6-9CCP6-7BKTT-D3WVR
Pro: W269N-WFGWX-YVC9B-4J6C9-T83GX
Pro N: MH37W-N47XK-V7XM9-C7227-GCQG9
Education: NW6C2-QMPVW-D7KKK-3GKT6-VCFB2
Education N: 2WH4N-8QGBV-H22JP-CT43Q-MDWWJ
Enterprise: NPPR9-FWDCX-D2C8J-H872K-2YT43
Enterprise N: DPH2V-TTNVB-4X9Q3-TJR4H-KHJW4
```

## Definir servidor KMS
```
Use o comando “slmgr /skms kms8.msguides.com” para se conectar ao meu servidor KMS.
slmgr /skms kms8.msguides.com
```

## Ative seu Windows
```
O último passo é ativar seu Windows usando o comando “slmgr /ato”.
slmgr /ato
```

If you see the error 0x80070005, it means the server is busy. Please try the command “ato” again until you succeed.

