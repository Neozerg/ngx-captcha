[![npm version](https://badge.fury.io/js/ngx-captcha.svg)](https://badge.fury.io/js/ngx-captcha)
[![Build Status](https://api.travis-ci.org/Enngage/ngx-captcha.svg?branch=master)](https://travis-ci.org/Enngage/ngx-captcha)
[![NPM](https://nodei.co/npm/ngx-captcha.png?mini=true)](https://nodei.co/npm/ngx-captcha/)

## Angular Captcha

Google reCaptcha implementation for Angular 5 and beyond. 

## Installation

```javascript
npm install ngx-captcha
```

Import `NgxCaptchaModule ` to your module (i.e. `AppModule`)

```javascript
import { NgModule } from '@angular/core';
import { NgxCaptchaModule } from 'ngx-captcha';

@NgModule({
  imports: [
    NgxCaptchaModule
  })

export class AppModule { }
```

## Usage

### reCaptcha2

```html
<ngx-recaptcha2
  [siteKey]="siteKey"
  [size]="size"
  [hl]="lang"
  [theme]="theme"
  [type]="type"
  (expire)="handleExpire()"
  (load)="handleLoad($event)"
  (success)="handleSuccess($event)">
</ngx-recaptcha2>
```

### Invisible captcha

```html
<ngx-invisible-recaptcha
  [siteKey]="invisibleCaptchaSiteKey"
  [type]="type"
  [badge]="badge"
  (load)="handleLoad($event)"
  (success)="handleSuccess($event)">
</ngx-invisible-recaptcha>
```

For more details please visit [https://enngage.github.io/ngx-captcha/](https://enngage.github.io/ngx-captcha/)