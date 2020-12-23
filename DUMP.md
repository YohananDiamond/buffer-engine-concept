# DUMP

* Override default versions of a plugin - some random javascript
  plugin that comes with the distribution:
  
  ```scheme
  ;; Overrides default ft-javascript (from /usr/lib/bfe/distro/plugins/ft-javascript)
  (register-module 'ft-javascript
   :path "/usr/lib/bfe/custom-packages/plugins/ft-javascript"
   :load #f)
  ```
