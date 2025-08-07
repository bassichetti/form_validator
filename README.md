# 📧 Form Validator - Flutter Email Validation

Um projeto Flutter que demonstra como implementar validação robusta de formulário para campos de email com interface moderna e experiência do usuário otimizada.

## 🔥 **Funcionalidades Implementadas**

### **1. Validação de Email Robusta**
- ✅ Verificação se o campo não está vazio
- ✅ Validação usando regex para formato correto de email
- ✅ Mensagens de erro personalizadas em português
- ✅ Suporte para diferentes formatos de email válidos

### **2. Interface de Usuário Intuitiva**
- 📱 Campo de texto específico para email com teclado adequado
- 🎯 Ícone de email no campo para melhor UX
- 🎨 Design moderno seguindo Material Design
- 📋 Card informativo com regras de validação claras
- 🎨 AppBar estilizada com cores consistentes

### **3. Validação em Tempo Real**
- ⚡ `AutovalidateMode.onUserInteraction` - valida enquanto o usuário digita
- 💬 Feedback imediato visual para erros
- ✅ SnackBar de sucesso quando o email é válido
- 🚨 Mensagens de erro instantâneas

### **4. Características Técnicas**
- 🔄 Uso correto de `GlobalKey<FormState>` para gerenciar o formulário
- 🧹 Dispose adequado do controller para evitar memory leaks
- 🎯 Função de validação reutilizável `_validateEmail()`
- 📱 Layout responsivo com padding e espaçamentos adequados
- 🏗️ Arquitetura limpa e bem estruturada

### **5. Experiência do Usuário**
- 🎨 AppBar com título descritivo
- 📝 Instruções claras sobre as regras de validação
- 🎯 Botão destacado para submeter o formulário
- 💚 Feedback visual de sucesso em verde
- 🔴 Mensagens de erro em vermelho para contraste

## 🚀 **Como Executar o Projeto**

### Pré-requisitos
- Flutter SDK instalado
- Dart SDK
- Editor de código (VS Code, Android Studio, etc.)

### Passos para execução

1. **Clone o repositório:**
```bash
git clone https://github.com/bassichetti/form_validator.git
cd form_validator
```

2. **Instale as dependências:**
```bash
flutter pub get
```

3. **Execute o projeto:**
```bash
flutter run
```

## 📱 **Funcionalidades da Interface**

### Tela Principal
- **Campo de Email**: TextFormField com validação em tempo real
- **Botão de Validação**: Submete o formulário e exibe resultado
- **Card de Regras**: Mostra as regras de validação aplicadas
- **Feedback Visual**: SnackBar para sucesso e mensagens de erro

### Validações Implementadas

| Validação | Descrição | Mensagem de Erro |
|-----------|-----------|------------------|
| Campo Vazio | Verifica se o campo não está vazio | "Por favor, insira um email" |
| Formato Email | Valida formato usando regex | "Por favor, insira um email válido" |
| Caracteres Especiais | Aceita caracteres válidos em emails | Validação automática |
| Domínio | Verifica presença de @ e domínio válido | Incluído na validação geral |

## 🛠️ **Tecnologias Utilizadas**

- **Flutter**: Framework de desenvolvimento mobile
- **Dart**: Linguagem de programação
- **Material Design**: Sistema de design do Google
- **RegExp**: Para validação de padrões de email
- **TextFormField**: Widget especializado para formulários

## 📝 **Estrutura do Código**

```
lib/
└── main.dart                 # Arquivo principal com toda a lógica
    ├── MainApp               # Widget principal da aplicação
    ├── EmailFormPage         # Página do formulário
    └── _EmailFormPageState   # Estado da página com validações
```

## 🎯 **Padrão de Validação Email**

O projeto utiliza a seguinte expressão regular para validar emails:

```dart
final emailRegExp = RegExp(
  r'^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$',
);
```

Esta regex valida:
- Caracteres alfanuméricos, pontos, underscores, percentuais, mais e hífen antes do @
- Símbolo @ obrigatório
- Domínio com caracteres alfanuméricos, pontos e hífen
- Extensão de domínio com pelo menos 2 caracteres

## 🤝 **Contribuindo**

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📄 **Licença**

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👨‍💻 **Autor**

Desenvolvido por **bassichetti**

---

⭐ Se este projeto te ajudou, não esqueça de dar uma estrela!
