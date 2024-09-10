This is a fork of:

- [npm @zendostrike/jspdf-html2canvas-pro](https://www.npmjs.com/package/@zendostrike/jspdf-html2canvas-pro)
- [GitHub: zendostrike/jsPDF-html2canvas-pro](https://github.com/zendostrike/jsPDF-html2canvas-pro)

to fix the compilation error

```error
File '.../node_modules/@zendostrike/jsPDF-html2canvas-pro/types/index.d.ts' is not a module.
```

by changing `/types/index.d.ts` so the module name...

```typescript
declare module "jspdf" {
```

...now matches the npm package name

```typescript
declare module "@zendostrike/jsPDF-html2canvas-pro" {
```

---

zendostrike's ReadMe:

> [!CAUTION]
> Do not use this on a production environment

# jspdf-html2canvas-pro

[JsPDF](https://github.com/parallax/jsPDF) fork but using [html2canvas-pro](https://www.npmjs.com/package/html2canvas-pro). This is a temporary workaround for this [issue](https://github.com/parallax/jsPDF/issues/3748).

I created this repo only to test jsPDF on my local environment.