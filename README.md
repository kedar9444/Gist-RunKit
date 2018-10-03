# Angular Gist RunKit

![](https://firebasestorage.googleapis.com/v0/b/angularpoc-f717b.appspot.com/o/packages%2Fgist-runkit%2Fngx-gist-runkit-logo.png?alt=media&token=96bd676d-44b0-4731-8db0-2ae03bfb41ad)

Gist RunKit combines the power of Github Gist with RunKit.

## Source Code

[Gist-RunKit website](https://kedar9444.github.io/Angular-Gist-RunKit)


[Gist-RunKit source code ](https://github.com/kedar9444/Gist-RunKit)


[Gist-RunKit npm](https://www.npmjs.com/package/ngx-gist-runkit)

## Install

Install the package.

```sh
$ npm i -s ngx-gist-runkit
```

Add the RunKit embed library to your index page:

**`src/index.html`**
```html
<head>
    ...
    <script src="https://embed.runkit.com"></script>
    ...
</head>
```

Whitelist `angular-runkit` in your System.js config:

**`src/systemjs.config.js`** (if applicable)
```js
map: {
    ...
    'angular-runkit': 'npm:angular-runkit/dist/index.js',
    ...
}
```

Declare the component in your module:

**`src/app/app.module.ts`**
```ts
import { NgxGistRunkitModule } from 'ngx-gist-runkit'

...

@NgModule({
	...
	imports: [
		...
		NgxGistRunkitModule,
		...
	],
	...
})
```

## Usage

```html
<app-ngx-gist-runkit [gistId]="gistId" [gistFileName]="gistFileName" ></app-ngx-gist-runkit>
```


Don't forget to check out the [RunKit embed docs](https://runkit.com/docs/embed#options).

## Inputs

### source : string

Basically there are two inputs one is [gistId] and second is [gistFileName].

**`[gistId]`** : is the id present after you username when you open your gist on github.

**`[gistFileName]`** : Before creating any Gist  github asks for the filename you have to enter the same.

Please check below image for more details.

```html
<app-ngx-gist-runkit [gistId]="gistId" [gistFileName]="gistFileName" ></app-ngx-gist-runkit>
```
