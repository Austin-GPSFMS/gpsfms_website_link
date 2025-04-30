geotab.addin.customButton = function(api, state) {
  return {
    initialize: function(api, state, callback) {
      const btn = document.createElement('button');
      btn.innerText = 'Camera Solutions';
      btn.style.marginLeft = '10px';
      btn.className = 'button';

      btn.onclick = function() {
        window.open('https://www.gpsfms.com/geotab-camera-solutions', '_blank');
      };

      const observer = new MutationObserver(() => {
        const container = document.querySelector('.pageHeader .pageTitle');
        if (container && !document.getElementById('cameraSolutionsButton')) {
          btn.id = 'cameraSolutionsButton';
          container.appendChild(btn);
        }
      });

      observer.observe(document.body, { childList: true, subtree: true });

      callback();
    },
    focus: function() {},
    blur: function() {}
  };
};
