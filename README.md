# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type-aware lint rules:

```js
export default tseslint.config({
  extends: [
    // Remove ...tseslint.configs.recommended and replace with this
    ...tseslint.configs.recommendedTypeChecked,
    // Alternatively, use this for stricter rules
    ...tseslint.configs.strictTypeChecked,
    // Optionally, add this for stylistic rules
    ...tseslint.configs.stylisticTypeChecked,
  ],
  languageOptions: {
    // other options...
    parserOptions: {
      project: ['./tsconfig.node.json', './tsconfig.app.json'],
      tsconfigRootDir: import.meta.dirname,
    },
  },
})
```

You can also install [eslint-plugin-react-x](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-x) and [eslint-plugin-react-dom](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-dom) for React-specific lint rules:

```js
// eslint.config.js
import reactX from 'eslint-plugin-react-x'
import reactDom from 'eslint-plugin-react-dom'

export default tseslint.config({
  plugins: {
    // Add the react-x and react-dom plugins
    'react-x': reactX,
    'react-dom': reactDom,
  },
  rules: {
    // other rules...
    // Enable its recommended typescript rules
    ...reactX.configs['recommended-typescript'].rules,
    ...reactDom.configs.recommended.rules,
  },
})
```
## Example prompt
0.
```
https://ui.shadcn.com/docs/installation/vite
문서를 참고 해서 shadcn ui를 설치 하고, 많이 사용하는 주요 컴포넌트들을 되도록이면 많이 설치 해 줘
```
1.
```
https://www.figma.com/design/86ljHjpnEjb6wdWFaUCfS7/-%EA%B0%80%EC%9D%B4%EB%93%9C--%EB%82%B4%EB%B6%80%EB%AA%B0-%EA%B5%AC%EC%B6%95-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8?node-id=75-2293&m=dev

---
figma mcp를 이용해서 화면을 읽고, src/components/alert-config.tsx 파일을 만들고, 컴포넌트를 만들어줘.
컴포넌트는 app.tsx 화면에 출력 해 줘
```

2.
```
https://www.figma.com/design/86ljHjpnEjb6wdWFaUCfS7/-%EA%B0%80%EC%9D%B4%EB%93%9C--%EB%82%B4%EB%B6%80%EB%AA%B0-%EA%B5%AC%EC%B6%95-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8?node-id=52-446&t=BCGm5X5XzxNyTGSl-4
---
위 피그마 화면을 mcp로 읽어 들이고, 컴포넌트로 만들고, app.tsx 파일에 추가 해 줘
```

