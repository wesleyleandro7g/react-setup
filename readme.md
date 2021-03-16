# Setup para projetos React criados utilizando o "create next-app"

### **1 - Intale o Typescript como dependencia de desenvolvimento**

    yarn add typescript @types/react @types/node -D

### **2 - Execute o projeto para que seja criado o arquivo "tsconfig.json"**

### **3 - Instale o eslint como dependencia de desenvolvimento e o inicie**

    yarn add eslint -D
    yarn eslint --init

### **4 - Instale o prettier**

    yarn add prettier eslint-plugin-prettier eslint-config-prettier -D

### **5 - Configure o .eslintrc.json**

#### 5.1 Adicione as extensões

    'plugin:@typescript-eslint/recommended',
    'prettier/@typescript-eslint',
    'prettier/standard',
    'prettier/react'

#### 5.2 Adicione o plugin

    'prettier'

#### 5.3 Adicione as regras

    'prettier/prettier': 'error',
    'space-before-function-paren': 'off',
    'react/prop-types': 'off',
    'react-hooks/rules-of-hooks': 'error',
    'react-hooks/exhaustive-deps': 'warn'

### Crie um arquivo ".prettierignore"

#### Adcione os arquivos/pastas

    node_modules
    .next ou build
    /*.js

### Crie um arquivo chamado prettier.config.js

#### Exporte as configurações

    semi: false,
    singleQuote: true,
    arrowParens: 'avoid',
    trailingComma: 'none',
    endOfLine: 'auto'