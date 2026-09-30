<h1><p align="center">Navegadores</p></h1>

#### [Tor Browser](https://www.torproject.org/)
**Tor Browser** é um navegador focado em anonimato extremo que utiliza a rede Tor para rotear o tráfego através de múltiplos nós, ocultando o endereço IP e a identidade do usuário de forma muito robusta.

#### [Mullvad Browser](https://mullvad.net/browser)
**Mullvad Browser** é uma versão focada em privacidade que importa as tecnologias de "anti-fingerprinting" (anti-impressão digital) do Tor para sua navegação, mas sem o uso da rede Tor, sendo ideal para ser usado com uma VPN ou conexão padrão.

#### [Brave](https://brave.com/)
**Brave Browser** é um navegador privado por padrão baseado no Chromium, que bloqueia anúncios e rastreadores de forma nativa, oferecendo uma experiência familiar e com alta compatibilidade com sites.

<details markdown="block">
<summary>⚙️ Configuração recomendada do Brave Desktop</summary>

---

Essas opções podem ser encontradas em ☰ → Configurações.

⬜ **ESCUDOS**<br>
Brave inclui algumas medidas anti-impressão digital em seu recurso [Escudos](https://support.brave.com/hc/articles/360022973471-What-is-Shields). Sugiro configurar essas opções [globalmente](https://support.brave.com/hc/articles/360023646212-How-do-I-configure-global-and-site-specific-Shields-settings) em todas as páginas que você visita.

As opções do Escudo podem ser rebaixadas por site, conforme necessário, mas por padrão recomendo definir o seguinte:
- [x] Selecione **Agressivo** em _Rastreadores & bloqueio de anúncios_

<details markdown="block">
<summary>⚠️ Usar listas de filtros padrão</summary>

> O Brave permite que você selecione filtros de conteúdo adicionais na página interna `brave://adblock`. Aconselho não usar esse recurso; em vez disso, mantenha as listas de filtros padrão. Usar listas extras fará com que você se destaque de outros usuários do Brave e também poderá aumentar a superfície de ataque se houver uma exploração no Brave e uma regra maliciosa for adicionada a uma das listas que você usa.

---
</details>

- [x] Selecione **Rigorosa** em _Fazer upgrade das conexões para HTTPS_
- [x] Selecione **Bloquear scripts** (Opcional)
> Esta opção desativa o JavaScript, o que quebrará muitos sites. Para corrigi-los, você pode definir exceções por site clicando no ícone Escudo na barra de endereço e desmarcando essa configuração em _Opções avançados_.
- [x] Verifique **Bloquear impressões digitais**
- [x] Selecione **Bloquear cookies de terceiros**
- [x] Verifique **Esqueça de mim quando fechar este site**
> Se desejar permanecer conectado a um site específico que você visita com frequência, você pode definir exceções por site clicando no ícone Escudo na barra de endereço e desmarcando essa configuração em _Opções avançados_.
- [ ] Desmarque todos os componentes de mídia social

⬜ **PRIVACIDADE E SEGURANÇA**<br>
- [x] Selecione **Não permitir que os sites usem a otimização de JavaScript** em _Segurança_ → _Gerenciar a otimização e segurança de JavaScript_
> Desativar o otimizador V8 reduz sua superfície de ataque desativando [algumas](https://grapheneos.social/@GrapheneOS/112708049232710156) partes da compilação JavaScript Just-In-Time (JIT).
- [x] Selecione **Remover automaticamente as permissões de sites não usados** em _Configurações de site e segurança (escudos)_
- [x] Selecione **Desativar UDP não proxy** na [Política de manuseio de IP do WebRTC](https://support.brave.com/hc/articles/360017989132-How-do-I-change-my-Privacy-Settings#webrtc)
- [ ] Desmarque **Use os serviços do Google para receber mensagens push**
- [x] Selecione **Redirecionar automaticamente páginas de AMP**
- [x] Selecione **Redirecionar URLs de rastreamento automaticamente**
- [x] Selecione **Impedir que sites criem impressões digitais minhas com base nas minhas preferências de idioma**

⬜ **JANELAS TOR**<br>
[Janela privada com o Tor](https://support.brave.com/hc/articles/360018121491-What-is-a-Private-Window-with-Tor-Connectivity) permite que você roteie seu tráfego pela rede Tor no Private Windows e acesse os serviços .onion, que podem ser úteis em alguns casos. No entanto, o Brave não é tão resistente à impressão digital quanto o navegador Tor, e muito menos pessoas usam o Brave com Tor, então você vai se destacar. Se o seu modelo de ameaça exigir forte anonimato, use o navegador [Tor]().

⬜ **COLETA DE DADOS**<br>
- [ ] Desmarque **Permitir a análise de produtos com preservação da privacidade (P3A)**
- [ ] Desmarque **Enviar automaticamente um ping diário de uso ao Brave**
- [ ] Desmarque **Enviar relatórios de diagnóstico automaticamente**

⬜ **WEB3**<br>
Os recursos Web3 do Brave podem potencialmente aumentar a impressão digital e a superfície de ataque do seu navegador. A menos que você use algum desses recursos, eles devem ser desativados
- [x] Selecione **Extensões (sem fallback)** em _Carteira Ethereum padrão_
- [x] Selecione **Extensões (sem fallback)** em _Carteira Solana padrão_

⬜ **MECANISMO DE PESQUISA**<br>
- [ ] Desmarque **Melhores sugestões de pesquisa**
> As sugestões de pesquisa enviam tudo o que você digita na barra de endereço para o mecanismo de pesquisa padrão, independentemente de você enviar uma pesquisa real. Desativar sugestões de pesquisa permite que você controle com mais precisão quais dados você envia ao seu provedor de mecanismos de pesquisa.

⬜ **EXTENSÕES**<br>
- [ ] Desmarque todas as extensões integradas que você não usa

⬜ **SISTEMA**<br>
- [ ] Desmarque **Continuar executando os aplicativos em segundo plano quando o Brave for fechado**
> Esta opção não está presente em todas as plataformas.

⬜ **BRAVE SYNC**<br>
[Brave Sync](https://support.brave.com/hc/articles/360059793111-Understanding-Brave-Sync) permite que seus dados de navegação (histórico, favoritos, etc.) estejam acessíveis em todos os seus dispositivos sem a necessidade de uma conta e os protege com a criptografia de ponta a ponta.

⬜ **RECOMPENSAS BRAVE**<br>
**Recompensas Brave** permite que você receba a criptomoeda Basic Attention Token (BAT) por executar determinadas ações no Brave. Ele depende de uma conta de custódia e KYC (Know Your Costumer) de um número selecionado de provedores. Não recomendo o BAT como uma **criptomoeda privada**, nem recomendo o uso de uma **carteira de custódia**, por isso desencorajo o uso desse recurso.

⬜ **CARTEIRA BRAVE**<br>
**Carteira Brave** opera localmente no seu computador, mas não oferece suporte a nenhuma criptomoeda privada, por isso desencorajo o uso desse recurso também.

---
</details>

<details markdown="block">
<summary>⚙️ Configuração recomendada do Brave Mobile</summary>

---

Essas opções podem ser encontradas em ⋮ → Configurações → Proteções do Brave e privacidade.

⬜ **PADRÕES GLOBAIS DO BRAVE SHIELDS**<br>
Brave inclui algumas medidas anti-impressão digital em seu recurso [Escudos](https://support.brave.com/hc/articles/360022973471-What-is-Shields). Sugiro configurar essas opções [globalmente](https://support.brave.com/hc/articles/360023646212-How-do-I-configure-global-and-site-specific-Shields-settings) em todas as páginas que você visita.

As opções do Escudo podem ser rebaixadas por site, conforme necessário, mas por padrão recomendo definir o seguinte:
- [x] Selecione **Agressivo** em _Bloquear rastreadores e anúncios_
- [x] Selecione **Redirecionar automaticamente páginas de AMP**
- [x] Selecione **Redirecionar URLs de rastreamento automaticamente**
- [x] Selecione **Estrito** em _Fazer upgrade das conexões para HTTPS_
- [x] Selecione **Bloquear scripts** (Opcional)
> Esta opção desativa o JavaScript, o que quebrará muitos sites. Para corrigi-los, você pode definir exceções por site clicando no ícone Escudo na barra de endereço e desmarcando essa configuração em _Opções avançados_.
- [x] Selecione **Bloquear cookies de terceiros** em _Bloquear cookies_
- [x] Selecione **Bloquear impressões digitais**
- [x] Selecione **Evite impressões digitais por meio das configurações de idioma**

<details>
<summary>⚠️ Usar listas de filtros padrão</summary>

> O Brave permite que você selecione filtros de conteúdo adicionais no menu **Filtragem de conteúdo** ou na página interna `brave://adblock`. Não recomendo o uso desse recurso; em vez disso, mantenha as listas de filtros padrão. O uso de listas adicionais fará com que você se destaque dos demais usuários do Brave e também poderá aumentar a superfície de ataque caso haja uma vulnerabilidade no Brave e uma regra maliciosa seja adicionada a uma das listas que você utiliza.

---
</details>

- [x] Selecione **Abas so site fechadas** em _Destruir_

⬜ **OUTRAS CONFIGURAÇÕES DE PRIVACIDADE**<br>
- [x] Selecione **Sem proteção** em _Navegação Segura_
- [x] Selecione **Desativar UDP não proxy** em [Política de manuseio de IP do WebRTC](https://support.brave.com/hc/articles/360017989132-How-do-I-change-my-Privacy-Settings#webrtc)
- [ ] Desmarque **Permitir que os sites verifiquem se você tem formas de pagamento salvas**
- [x] Selecione **Do no speed up sites with Brave's V8** em _Otimização e segurança de JavaScript_
- [x] Selecione **Fechar as guias ao sair**
- [ ] Desmarque **Enviar relatórios de diagnóstico automaticamente**
- [ ] Desmarque **Enviar automaticamente um ping diário de uso ao Brave**
- [ ] Desmarque **Autorizar pesquisas Brave**

⬜ **LEO AI**<br>
- [ ] Desmarque **Exibir sugestões de preenchimento automático na barra de endereço**

⬜ **MECANISMOS DE PESQUISA**<br>
- [ ] Desmarque **Mostrar sugestões de navegador**

⬜ **BRAVE SYNC**<br>
[Brave Sync](https://support.brave.com/hc/articles/360059793111-Understanding-Brave-Sync) permite que seus dados de navegação (histórico, favoritos, etc.) estejam acessíveis em todos os seus dispositivos sem a necessidade de uma conta e os protege com a criptografia de ponta a ponta.

---
</details>

#### [Firefox](https://firefox.com/)
**Firefox Browser** é um navegador de código aberto e independente (com seu próprio motor, o Gecko), conhecido por ser altamente personalizável e oferecer um equilíbrio entre privacidade, extensões e uso para o usuário geral.

<details markdown="block">
<summary>⚙️ Configuração recomendada do Firefox</summary>

---

Essas opções podem ser encontradas em ☰ → Configurações.

⬜ **PESQUISAR**<br>
- [ ] Desmarcar **Sugestões de mecanismos de pesquisa**

⬜ **PRIVACIDADE E SEGURANÇA → PROTEÇÃO APRIMORADA CONTRA RASTREAMENTO**<br>
- [x] Selecione **Rigoroso** em _Proteção aprimorada contra rastreamento_

Isso protege você bloqueando rastreadores de mídia social, scripts de impressão digital (observe que isso não protege você de _todas_ as impressões digitais), criptomineradores, cookies de rastreamento entre sites e algum outro conteúdo de rastreamento. O ETP protege contra muitas ameaças comuns, mas não bloqueia todos os caminhos de rastreamento porque foi projetado para ter impacto mínimo ou nenhum na usabilidade do site.

⬜ **DADOS DE NAVEGAÇÃO**<br>
Se você quiser permanecer conectado a sites específicos, poderá permitir exceções em **Dados de navegação → Gerenciar exceções...**
- [x] Selecione **Limpar cookies e dados de sites sempre que fechar o Firefox**

Isto protege-o de cookies persistentes, mas não o protege contra cookies adquiridos durante qualquer sessão de navegação. Quando isso estiver ativado, será possível limpar facilmente os cookies do seu navegador simplesmente reiniciando o Firefox. Você pode definir exceções por site, se desejar permanecer conectado a um site específico que visita com frequência.

⬜ **DNS SOBRE HTTPS**<br>
- [x] Selecione **Personalizado** em _Escolher provedor_ escolha um provedor adequado

O **Personalizado** impõe o uso de DNS sobre HTTPS, e um aviso de segurança será exibido se o Firefox não conseguir se conectar ao seu resolvedor de DNS seguro ou se o seu resolvedor de DNS seguro disser que os registros do domínio que você está tentando acessar não existem. Isso impede que a rede à qual você está conectado faça o downgrade secreto da segurança do seu DNS.

⬜ **CONEXÃO E SEGURANÇA DE SOFTWARE**<br>
- [x] Selecione **Ativar o modo somente HTTPS em todas as janelas**

Isso evita que você se conecte involuntariamente a um site em HTTP de texto simples. Sites sem HTTPS são incomuns hoje em dia, então isso deve ter pouco ou nenhum impacto na sua navegação diária.

⬜ **PERMISSÕES E DADOS**<br>
- [ ] Desmarcar **Enviar dados técnicos e de interação para a Mozilla**
- [ ] Desmarcar **Permitir recomendações personalizadas de extensões**
- [ ] Desmarcar **Permitir que o Firefox execute estudos de funcionalidades**
- [ ] Desmarcar **Permitir que o Firefox melhore funcionalidades, desempenho e estabilidade entre uma atualização e outra**
- [ ] Desmarcar **Enviar ping de uso diário para a Mozilla**
- [ ] Desmarcar **Enviar relatórios de falhas automaticamente**

De acordo com a política de privacidade da Mozilla para o Firefox:
> Firefox sends data about your Firefox version and language; device operating system and hardware configuration; memory, basic information about crashes and errors; outcome of automated processes like updates, safebrowsing, and activation to us. When Firefox sends data to us, your IP address is temporarily collected as part of our server logs.

⬜ **CONTA E SINCRONIZAÇÃO → SINCRONIZAÇÃO**<br>
O [Firefox Sync](https://hacks.mozilla.org/2018/11/firefox-sync-privacy) permite que seus dados de navegação (histórico, favoritos, etc.) estejam acessíveis em todos os seus dispositivos e os protege com o E2EE.

Além disso, o serviço Contas Mozilla coleta [alguns dados técnicos](https://mozilla.org/privacy/mozilla-accounts). Se você usar uma conta Mozilla, poderá cancelar:

1. Abra as [configurações do seu perfil](https://accounts.firefox.com/settings#data-collection)
2. Desmarque **Contas Mozilla** em _Coleta e uso de dados_

---
</details>

<h1><p align="center">Extensões</p></h1>
