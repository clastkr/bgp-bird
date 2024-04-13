BIRD Setup Guideline
=============

Information
-------------

> VM OS: CentOS 7 x64
> 
> VM IPv4: 207.246.123.123
> 
> VM IPv6: 2001:19f0:1000:7552:5400:04ff:fe9f:1234
>
> ASN: 216362
>
> Vultr ASN: 64515
> 
> Vultr IPv4: 169.254.169.254
> 
> Vultr IPv6: 2001:19f0:ffff::1
> 
> Vultr BGP Password: bgppw
> 
> Vultr Multihop: 2


Anycast IP command
-------------

```
sudo yum install epel-release -y
sudo yum update -y
sudo yum install bird -y
sudo systemctl start bird
sudo systemctl enable bird

ip link show
ip addr add [배포하고자 하는 IPv4 또는 IPv6 예)141.11.245.100/24] dev [네틑워크 인터페이스 명 예)eth0]
```

