# Tying your module to your Addons account

In order to tie your module to you PrestaShop Addons account, you simply need to add your Addons key to the module's constructor:

```
  public function __construct()
  {
    $this->name = 'mymodule';
    $this->tab = 'front_office_features';
    $this->version = '1.0.0';
    $this->author = 'Firstname Lastname';
    $this->need_instance = 0;
    $this->ps_versions_compliancy = array('min' => '1.6', 'max' => _PS_VERSION_);  
    $this->bootstrap = true;
    $this->module_key = '084fe8aecafea8b2f84cca493377eb9b';

(...)
```

The `module_key` can be found in your contributor account, in the module upload page.
