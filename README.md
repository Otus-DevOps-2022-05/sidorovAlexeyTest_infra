# sidorovAlexeyTest_infra
sidorovAlexeyTest Infra repository

Подключение в одну комманду:
В .ssh создаём файл config с содердимым:

Host someinternalhost
  HostName 10.128.0.17
  User appuser
  IdentityFile ~/.ssh/id_rsa
  Port 22

  ## sample for ProxyJump
  ProxyJump appuser@51.250.10.50

bastion_IP = 51.250.10.50
someinternalhost_IP = 10.128.0.17
