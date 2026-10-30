# DANI CREATOR — versão Firebase

App React + Firebase Firestore + Firebase Storage. Atualizações em tempo real entre dispositivos.

## Configuração única
1. Entre em https://console.firebase.google.com/ com sua conta Google e crie um projeto chamado `dani-creator`.
2. Adicione um aplicativo Web (ícone `</>`) e copie os campos do objeto `firebaseConfig`.
3. No DANI CREATOR, abra o ícone de nuvem e cole os seis campos: `apiKey`, `authDomain`, `projectId`, `storageBucket`, `messagingSenderId`, `appId`.
4. No Firebase Console, crie o Firestore Database em modo de produção e cole as regras do arquivo `firebase.rules.txt` na aba Rules.
5. Ative Storage e cole as regras de Storage do mesmo arquivo.

Após essa configuração inicial, o app reconecta automaticamente nesse navegador e sincroniza projetos em tempo real.

## Atenção sobre acesso público
As regras fornecidas permitem que qualquer pessoa que tenha o link do app leia, crie, altere e exclua projetos e arquivos. Isso atende ao pedido de edição por qualquer pessoa com o link, mas o link não é uma senha. Não guarde informações privadas. Para maior segurança, configure Firebase Authentication e regras por usuário.

## Publicar
Hospede o conteúdo deste projeto em um host estático que suporte SPA. Comandos: `npm install` e `npm run build`; pasta publicada: `dist`.