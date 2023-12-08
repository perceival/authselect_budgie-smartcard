# authselect_budgie-smartcard
Tweaked authselect smartcard profile to work with Yubikeys (Fedora/Ultramarine).
An idea is:
- to be forced to logon using password to Budgie desktop since that is required to unlock keyring.
- to be able to unlock Budgie screen lock with Yubikey and PIN.
- to be able to use Yubikey without PIN for sudo and su.
- To support ssh -A and mDNS name resoultion.
Folder to be placed under /etc/authselect/custom and applied with the command:
sudo authselect  select 'custom/budgie-smartcard' 'with-pam-u2f' 'with-ssh-agent' 'with-mdns4'
