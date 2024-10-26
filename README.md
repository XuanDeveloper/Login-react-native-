# Login Screen - React Native

Este é um projeto de uma tela de login moderna e responsiva desenvolvida em React Native. O projeto implementa uma interface de usuário limpa e intuitiva com autenticação básica. 

## 🚀 Funcionalidades

- Interface moderna e minimalista
- Formulário de login com email e senha
- Autenticação básica
- Design responsivo
- Suporte a modo claro
- Feedback visual para o usuário
- Links para recuperação de senha e cadastro

## 📋 Pré-requisitos

- Node.js (versão 14 ou superior)
- npm ou yarn
- React Native CLI ou Expo CLI
- iOS Simulator ou Android Emulator (para desenvolvimento)

## 🔧 Instalação

1. Clone o repositório:
```bash
git clone [[url-do-seu-repositorio](https://github.com/XuanDeveloper/Login-react-native-)]
cd [Login-react-native-]
```

2. Instale as dependências:
```bash
npm install
# ou
yarn install
```

3. Execute o projeto:
```bash
# Para React Native CLI
npx react-native run-android
# ou
npx react-native run-ios

# Para Expo
expo start
```

## 📁 Estrutura do Projeto

```
src/
├── screens/
│   └── LoginScreen.js
├── components/
├── assets/
└── App.js
```

## 💻 Como Usar

1. Importe o componente LoginScreen:
```javascript
import LoginScreen from './src/screens/LoginScreen';
```

2. Use o componente em seu App.js:
```javascript
import React from 'react';
import LoginScreen from './src/screens/LoginScreen';

const App = () => {
  return <LoginScreen />;
};

export default App;
```


## ⚙️ Personalização

### Cores
Você pode modificar as cores do projeto alterando as variáveis no objeto `styles`:

```Typecript
const styles = StyleSheet.create({
  // ...
  loginButton: {
    backgroundColor: '#0066FF', // Altere para sua cor preferida
  },
  // ...
});
```

### Textos
Para alterar os textos para português ou outro idioma, modifique as strings no componente:

```Typecript
<Text style={styles.title}>Bem-vindo de volta</Text>
<Text style={styles.subtitle}>Por favor, faça login para continuar</Text>
```

## 🔄 Conectando com Backend

Para conectar com seu backend, modifique a função `handleLogin`:

```Typecript
const handleLogin = async () => {
  try {
    const response = await fetch('sua-api/login', {
      method: 'POST',
      headers: {
        'Content-Type': 'application/json',
      },
      body: JSON.stringify({
        email,
        password,
      }),
    });
    
    const data = await response.json();
    // Trate a resposta conforme necessário
  } catch (error) {
    console.error(error);
  }
};
```

## 📱 Sugestões de Melhorias

1. **Validação de Formulário**
   - Adicionar validação de email
   - Validação de força da senha
   - Mensagens de erro personalizadas

2. **UX/UI**
   - Adicionar indicador de loading
   - Animações de transição
   - Suporte a tema escuro
   - Máscaras nos inputs

3. **Segurança**
   - Implementar autenticação JWT
   - Adicionar autenticação biométrica
   - Armazenamento seguro de tokens

4. **Funcionalidades**
   - Persistência de login
   - Recuperação de senha
   - Cadastro de novos usuários

## 🤝 Contribuindo

1. Faça um Fork do projeto
2. Crie uma Branch para sua Feature (`git checkout -b feature/AmazingFeature`)
3. Faça o Commit de suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Faça o Push para a Branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 📞 Suporte

Para suporte, envie um email para [seu-email@exemplo.com] ou abra uma issue no repositório.

## ✨ Agradecimentos

- Design inspirado em tendências modernas de UI/UX
- Comunidade React Native
- Contribuidores do projeto

---

Desenvolvido com ❤️ por [https://github.com/XuanDeveloper]
Musica que estava tocando [https://open.spotify.com/intl-pt/track/4bMpS5EYjAPHhZRWoEu7EV?si=283cd1c4dee04906]
