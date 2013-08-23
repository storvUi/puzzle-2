
# 2
---

<h1>2222222222222222222</h2>


````javascript
seajs.use(['$', 'popup', 'puzzle'], function($, Popup, puzzle) {
  puzzle.init($('#container li'));

  $(document).keyup(function(e) {
    puzzle.push(e.which);
  });

  setTimeout(function() {
    $('#hint').show();
  },1000);

  new Popup({
    trigger: '#hint',
    align: {
      baseXY: ['100%', '50%'],
      selfXY: [0, '50%']
    },
    template: '<div class="hint-popup">支付宝前端类库</div>'
  }).render();
});

````
