# Mulesoft secure properties encryption with the cluster master key

Some of the properties holding secret information are encrypted with the
cluster master key. You can find the master key in Keepass under
Mulesoft folder.

There is a java jar file used to encrypt/decrypt.

Here is the jar file attached:

![](./media/image1.tmp)

To encrypt a secure property you will need:

  - java installed on the machine you are working on

  - download the jar file secure-properties-tool.jar

  - value of the property to be encrypted

  - the master cluster encryption key, separate for PRD and STG, you can
    find it in Keepass

Encryption of a property example:

java -cp ./secure-properties-tool.jar
com.mulesoft.tools.SecurePropertiesTool string encrypt Blowfish CBC
CLUSTER\_MASTER\_KEY\_NO\_QUOTES "VALUE\_TO\_BE\_ENCRYPTED"

Decryption of a property example: (you can use this to validate that the
encrypted property added to the build is correct, by trying to decrypt
it)

java -cp ./secure-properties-tool.jar
com.mulesoft.tools.SecurePropertiesTool string decrypt Blowfish CBC
CLUSTER\_MASTER\_KEY\_NO\_QUOTES "ALREADY\_ENCRYPTED\_VALUE"

**NOTE: If the password has "\!" in it, you will need to type "set +H"
on the terminal before you try to encrypt or decrypt.**
