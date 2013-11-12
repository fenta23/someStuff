someStuff
=========
var current = null;
document.body.addEventListener('click', function(ev) {
    if (ev.target.tagName === 'BUTTON') {
        if (current) {
            current.classList.remove('focus');
        }
        current = ev.target;
        current.classList.add('focus');
    }
}, false);
