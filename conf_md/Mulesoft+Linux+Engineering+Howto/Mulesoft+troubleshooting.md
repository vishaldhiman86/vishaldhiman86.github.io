# Mulesoft troubleshooting

## Mulesoft Access Troubleshooting for dev/qa cluster.

1.Checking for cluster pods

           sganga@DESKTOP-7QAAQI2:\~/mulesoft/tools$ kubectl get po -A  
           Unable to connect to the server: dial tcp 172.29.3.14:443:
i/o timeout

2.  Networking team confirms if the request is passing through firewall
for the IP's listed below

      [169.254.79.10](http://169.254.79.10),
[169.254.105.70](http://169.254.105.70))

3\. Update the Ip's in AWS security group to allow inbound traffic 

    SG Name:  eks-cluster-sg-rtf-dev-1512825132

    Ip Cidr Range: 169.254.79.10/32, port:443

                           169.254.105.70/32, port: 443

4\. Login to aws profile and switch context 

5\. Run kubectl get po -A
