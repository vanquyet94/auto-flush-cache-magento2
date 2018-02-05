Magento 2 module to automatically flush the cache whenever you save something in the System Configuration.

Step 1: Create folder app/VoolaTech/AutoFlushCache
Step 2: Download and extract 
Step 3: Start Module: php bin/magento setup:upgrade

This module listens to the event controller_action_postdispatch_adminhtml_system_config_save. Whenever it is called, it flushes the following caches:
* config
* block_html
* full_page
