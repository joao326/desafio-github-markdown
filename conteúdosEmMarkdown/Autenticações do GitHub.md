# Autenticações do GitHub
 
 

**>> NOME DE USUÁRIO E SENHA**
1. É considerada arriscada para informações sensíveis. 
2. Recomenda-se explorar outras opções mais seguras disponíveis.

**>> TOKENS DE ACESSO PESSOAL**
1. Os PATs (Tokens de Acesso Pessoal) são como senhas especiais que substituem o uso da senha normal ao acessar o GitHub pela API ou pela linha de comando. 
2. Você cria esse token nas configurações do GitHub e decide quais ações ele pode realizar em um repositório ou organização. 
3. Quando você usa a linha de comando do Git para trabalhar no GitHub, em vez de digitar seu nome de usuário e senha, você insere esse token para se autenticar.  
4. Torna a interação mais segura e prática.

**>> CHAVES SSH**
1. chaves especiais que ajudam as pessoas a se conectarem a computadores remotos de forma segura, sem precisar sempre digitar senha ou token.
2. É protegida por uma "frase secreta" para garantir ainda mais segurança.  
	- É possível configurar seu computador para usar essa chave automaticamente, ou digitar a "frase secreta" quando necessário.
3. É possível usar essas chaves em organizações que usam uma forma avançada de login. 
	-  Se a organização fornece certificados especiais, as pessoas podem usá-los para acessar os repositórios sem precisar adicionar nada à sua conta no GitHub.

**>> CHAVES DE IMPLEMENTAÇÃO**
1. Chaves especiais que permitem acesso a apenas um lugar específico no GitHub, como um cofre digital. 
2. No GitHub, a parte da chave que todos podem ver é conectada diretamente ao local desejado (um repositório), enquanto a parte secreta fica guardada no seu próprio computador.
3. Essas chaves são configuradas para permitir apenas leitura por padrão 
	1. você pode ver o que está dentro, mas não modificar nada. 
	2. Se quiser também fazer alterações, você pode configurar essas chaves para ter permissão de escrita, adicionando-as ao local específico (repositório). 
	3. São como chaves digitais que abrem a porta para um lugar específico no GitHub, e você decide se só quer olhar ou também mexer nas coisas.
## Opções de seguranças adicionais

**>> Autenticação de dois Fatores - 2FA**
1. adiciona uma camada extra de segurança quando você entra em sites ou aplicativos. 
	1. Além de digitar seu nome de usuário e senha, você precisa fornecer mais uma prova de que é realmente você.
	2. No caso do GitHub, essa prova extra geralmente é um código gerado por um aplicativo no seu celular ou enviado por mensagem de texto. 
2. Depois de ativar a 2FA, sempre que alguém tenta entrar na sua conta, o GitHub pede esse código adicional. 

**>> SSO do SAML**
1. Permite controlar o acesso aos recursos da organização de maneira centralizada. 
2. Em vez de usar senhas, os usuários são redirecionados para um sistema central de login (IdP), como o Microsoft Entra ID ou Okta. Após autenticados lá, eles retornam ao GitHub com acesso aos recursos da organização.
3. Facilita o gerenciamento, pois os proprietários da organização controlam quem pode acessar o quê. 
4. O GitHub suporta vários provedores populares, como:
	1. Active Directory;
	2. Microsoft Entra ID;
	3. Okta. 

**>>** **LDPA**
1. Protocolo usado para acessar e organizar informações em diretórios, especialmente em grandes empresas. 
2. No contexto do GitHub Enterprise Server, ele permite integrar e gerenciar centralmente o acesso aos repositórios usando contas existentes.
3. O GitHub Enterprise Server é compatível com vários serviços LDAP conhecidos, como:
	1. Active Directory;
	2. Oracle Directory Server Enterprise Edition; 
	3. OpenLDAP;
	4. outros. 
4. Em resumo, o LDAP é uma ferramenta que ajuda na organização e controle de acesso em ambientes corporativos no GitHub.

## Links importantes
- [https://support.github.com/](https://support.github.com/)
- [https://docs.github.com/pt/authentication](https://docs.github.com/pt/authentication)