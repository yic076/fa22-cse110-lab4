1. line 9 prints `values added: 20`  
2. line 13 prints `values added: 20`
3. line 9 prints `values added: 20`  
4. line 13 returns an error because result is now defined using let, so it's scope is limited to the if statment. Line 13 is out side of it and therefore doesn't recognize result.
5. line 9 returns an error because result is now defined using const but line 7 tries to change it, which isn't allowed.
6. line 13 returns an error for the same reson as question 4. Both let and const are limited within their block.

