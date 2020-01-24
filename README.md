# DockerContentTrust
Docker Security using Signed Content trust


$ docker trust key generate penguin --dir ~/.docker/trust

$notary -d ~/.docker/trust key list

$ docker trust signer add --key ~/.docker/trust/marco.pub marco kumagaur/centosnew

$ notary -d ~/.docker/trust key list

$docker pull ubuntu

$docker tag ubuntu  kumagaur/centosnew:latest

$ docker trust sign marcofranssen/whalesay:latest


$docker trust inspect --pretty kumagaur/centosnew
