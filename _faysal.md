---
layout: post
title: This is my first blog post
---
## Faysal Ahmmad
```markdown

import { NgControl } from '@angular/forms';
import { Input, Directive } from '@angular/core';

@Directive({
  selector: '[disableControl]'
})
export class DisableControlDirective {

  @Input() set disableControl( condition: boolean ) {
    const action = condition ? 'disable' : 'enable';
    this.ngControl.control[action]();
  }

  constructor( private ngControl: NgControl ) {
  }

}
```
