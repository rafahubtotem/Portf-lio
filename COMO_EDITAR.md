# Como Editar Seu Portfólio

## 📝 Editando o Conteúdo

### Arquivo Principal de Dados
Todas as informações do portfólio estão centralizadas no arquivo:
```
src/data/portfolioData.js
```

### Seções Editáveis

#### 1. Informações Pessoais
```javascript
personal: {
  name: "[Seu Nome Completo]",
  tagline: "Sua tagline profissional",
  profileImage: "/src/assets/profile_placeholder.png", // Substitua pela sua foto
  email: "seuemail@exemplo.com",
  phone: "+55 (11) 99999-9999",
  linkedin: "https://linkedin.com/in/seuperfil",
  github: "https://github.com/seuperfil",
  website: "https://seusite.com"
}
```

#### 2. Experiências Profissionais
```javascript
experience: [
  {
    id: 1,
    company: "Nome da Empresa",
    position: "Seu Cargo",
    period: "Jan 2022 - Presente",
    description: "Descrição das suas responsabilidades e conquistas.",
    icon: "briefcase"
  }
  // Adicione mais experiências conforme necessário
]
```

#### 3. Formação Acadêmica
```javascript
education: [
  {
    id: 1,
    institution: "Nome da Instituição",
    course: "Nome do Curso",
    period: "2014 - 2018",
    honors: "Menções honrosas (opcional)",
    icon: "graduation-cap"
  }
]
```

#### 4. Projetos
```javascript
projects: [
  {
    id: 1,
    name: "Nome do Projeto",
    description: "Descrição detalhada do projeto",
    technologies: ["React", "Node.js", "MongoDB"],
    link: "https://github.com/seuprojeto",
    image: "/src/assets/project1.jpg" // Opcional
  }
]
```

#### 5. Habilidades
```javascript
skills: {
  design: [
    { name: "UI/UX Design", level: 95, icon: "palette" }
  ],
  frontend: [
    { name: "React", level: 92, icon: "react" }
  ],
  // ... outras categorias
}
```

## 🖼️ Substituindo Imagens

### Foto de Perfil
1. Coloque sua foto na pasta `src/assets/`
2. Atualize o caminho em `portfolioData.js`:
```javascript
profileImage: "/src/assets/sua_foto.jpg"
```

### Imagens de Projetos
1. Adicione as imagens na pasta `src/assets/`
2. Referencie no array de projetos:
```javascript
image: "/src/assets/nome_do_projeto.jpg"
```

## 🎨 Personalizando Cores

### Cores Principais
No arquivo `src/App.css`, você pode alterar as cores principais:
```css
:root {
  --portfolio-deep-blue: #060d2e;     /* Azul profundo */
  --portfolio-elegant-red: #a81f00;   /* Vermelho elegante */
  --portfolio-pure-white: #ffffff;    /* Branco puro */
}
```

## ⌨️ Navegação

### Controles Disponíveis
- **Setas do teclado**: ← → ↑ ↓ para navegar entre seções
- **Números 1-6**: Acesso direto às seções
- **Mouse**: Clique na navegação superior ou use as setas laterais
- **Indicadores**: Clique nos pontos na parte inferior

## 🚀 Executando Localmente

### Pré-requisitos
- Node.js instalado
- pnpm (gerenciador de pacotes)

### Comandos
```bash
# Instalar dependências
pnpm install

# Executar em modo desenvolvimento
pnpm run dev

# Construir para produção
pnpm run build
```

## 📱 Responsividade

O portfólio é totalmente responsivo e se adapta automaticamente a:
- Desktop (1024px+)
- Tablet (768px - 1023px)
- Mobile (até 767px)

## 🔧 Funcionalidades Especiais

### QR Code Automático
- Gerado automaticamente com a URL atual
- Atualiza dinamicamente quando hospedado

### Animações
- Efeitos hover nos cards
- Transições suaves entre seções
- Elementos geométricos animados
- Animações de entrada

### Acessibilidade
- Navegação por teclado
- Contraste adequado
- Estrutura semântica

## 💡 Dicas de Personalização

1. **Mantenha a consistência**: Use as mesmas cores e fontes em todo o portfólio
2. **Otimize imagens**: Use formatos web-friendly (WebP, JPG otimizado)
3. **Teste regularmente**: Verifique em diferentes dispositivos e navegadores
4. **Conteúdo conciso**: Mantenha textos claros e objetivos
5. **Links funcionais**: Sempre teste os links externos

## 📞 Suporte

Para dúvidas sobre personalização ou problemas técnicos, consulte a documentação do React e Tailwind CSS, ou entre em contato através dos canais de suporte.

