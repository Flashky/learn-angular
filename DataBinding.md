Databinding allows to seamlessly map data between the model and the html.

# Basic data binding

Go to your .ts file, and add a class attribute, for example:

```TypeScript
name = 'Bob';
```

Go to your .html file and add the following:

```html
<p>Hello, {{ name }}.</p>
```

Load your app, and you will see:
Hello, Bob.


# Directive based data binding

Directive based data binding is bidirectional: If you change your html, it will change your model, and if you change your model, it will change your html.

To use it, first you need to add a module to ``app.modules.ts``:

1. Add import: ``import { FormsModule } from '@angular/forms';``
2. Inside imports add: ``FormsModule``


Now go to your html and add the following:

```html
<input type="text" [(ngModel)]="name" />
```
