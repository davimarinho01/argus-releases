# Argus — versões publicadas

Este repositório guarda só os pacotes de cada versão do Argus, a ferramenta de auditoria de postura de segurança (somente leitura) da Argus Consultoria. O código-fonte fica num repositório privado.

## Como instalar

1. Abra a versão mais recente em **Releases**.
2. Baixe `Argus-<versão>-portatil.zip` e `SHA256SUMS.txt`.
3. Descompacte o zip e abra `Argus\Argus.exe`.

## Como atualizar

O Argus avisa sozinho quando há versão nova (Configurações › Atualização). Ele baixa o pacote, confere o código SHA-256 publicado em `SHA256SUMS.txt`, instala a versão nova numa pasta ao lado da atual e copia a pasta `dados` (perfis, auditorias e planos). A versão anterior continua no lugar até você apagá-la.

Para conferir um pacote baixado à mão, no PowerShell:

```powershell
Get-FileHash .\Argus-2.5.0-portatil.zip -Algorithm SHA256
```

O resultado precisa ser igual à linha correspondente em `SHA256SUMS.txt`.
