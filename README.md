# Script que substitui o CCleaner ( Script do BABOO versão 3.2a de 23/05/2024 )

> [!NOTE]  
> EXECUTAR O SCRIPT COMO ADMINISTRADOR

[➤ DOWNLOAD DIRETO E ATUALIZADO](https://www.baboo.com.br/script/atual)

![](https://i.imgur.com/GvkFWI0.png) Leia a matéria completa [clicando aqui](https://www.baboo.com.br/tutorial-windows/script-do-baboo-para-apagar-arquivos-temporarios/)

![](https://i.imgur.com/toQwUZE.png) Veja o vídeo [clicando aqui](https://www.youtube.com/watch?v=ybh0sXgzmXQ)

![](https://i.imgur.com/U8gYxcE.png)

---

Lista de arquivos que são removidos:

- Lixeira
- Pasta Windows/Temp
- Pasta de arquivos temporários de todos os usuários
- Arquivos de Log do Windows (Eventos e Minidump permanecem)
- Arquivos temporários dos primeiros 12 perfis dos navegadores Edge, Firefox, Chrome, Brave, Vivaldi e IE (cookies, histórico e senhas permanecem)
- Arquivos temporários do OneDrive
- Arquivos temporários do Media Cache files da Adobe
- Arquivos temporários do VMWare
- Arquivos temporários do TeamViewer
- Arquivos temporários de músicas do Spotify

> [!IMPORTANT]  
> Embora o código desse script permita apagar arquivos temporários de TODOS os usuários cadastrados no Windows, isso acontece SOMENTE se o usuário atual tiver acesso irrestrito às pastas dos demais usuários dentro de C:\Users. Se o usuário atual não consegue acessar as pastas dos demais usuários dentro de C:\Users, este script apaga apenas os arquivos temporários do usuário atual.Isso acontece apenas por questão de segurança, pois a remoção dos arquivos temporários dos demais usuários exige a mudança nas permissões de centenas ou milhares de pastas e arquivos dentro de C:\Usuarios.
> 
> Além dessa tarefa ser lenta, isso permitiria que o usuário atual também pudesse acessar aqueles arquivos, colocando em risco a segurança e privacidade dos dados dos demais usuários.

---

### O script em questão foi retirado do seguinte site:

🌐 https://www.baboo.com.br/script

📌 Não pretendo realizar modificações "agressivas" no script. Ele foi copiado integralmente do site original.

💡 **Quer contribuir com o script?** Entre em contato com o proprietário do script, enviando uma mensagem para o e-mail 📧 `aurelio@baboo.com.br`

🔗 [www.baboo.com.br/baboo](https://www.baboo.com.br/baboo)

---

### ✨ CONTRIBUIÇÕES

<details>
<summary><strong>Discord cache clear by <a href="https://github.com/ravenastar-js/Script-que-substitui-o-CCleaner/commit/ec366ce7e425ba67476c8caa21159b81e0625f03">@wellerychaves</a></strong></summary>

```batch
REM ******************* Discord *******************

taskkill /F /IM "Discord.exe"

for /d %%U in (C:\Users\*) do (
    del %%U\AppData\Roaming\discord\Cache\* /s /q
    del %%U\AppData\Roaming\discord\"Code Cache"\* /s /q
    del %%U\AppData\Roaming\discord\GPUCache\* /s /q
)

REM ******************* Discord PTB *******************

taskkill /F /IM "DiscordPTB.exe"

for /d %%U in (C:\Users\*) do (
    del %%U\AppData\Roaming\discordptb\Cache\* /s /q
    del %%U\AppData\Roaming\discordptb\"Code Cache"\* /s /q
    del %%U\AppData\Roaming\discordptb\GPUCache\* /s /q
)

REM ******************* Discord Canary *******************
taskkill /F /IM "DiscordCanary.exe"

for /d %%U in (C:\Users\*) do (
    del %%U\AppData\Roaming\discordcanary\Cache\* /s /q
    del %%U\AppData\Roaming\discordcanary\"Code Cache"\* /s /q
    del %%U\AppData\Roaming\discordcanary\GPUCache\* /s /q
)
```

</details>
