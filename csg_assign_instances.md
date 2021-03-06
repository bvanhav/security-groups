---



copyright:
  years: 2017, 2018
lastupdated: "2018-02-15"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}

# Assigning Instances to the Security Group
You can assign security group objects to instances in one of two ways:

## Using the Security Menu

1. From the **Security** tab on the [Customer Portal ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/){: new_window}, under **Network Security** select **Security Groups**.
2. Click the ![More icon](./images/more_icon.jpg) icon of the Security Group object you wish to assign instances to, then select **Manage Instances**.
3. Select the instance and interface to apply to the Security Group.

	![Security Menu Instance](./images/security_assign.jpg)

	In the figure, the "allow_icmp" Security Group (created in the [first step](csg_create.html)) is applied to the private interface (`10.0.2.219`) of "jpmongevsi4".

	Note how the **Attached Instances** count increased from `0` to `1`.

4. Click **Save** to apply the changes.

5. Reboot your instance.

	**NOTE:** This is a one-time-only step per network interface for instances not created with a security group.

## Using the Devices Menu

1. From the **Devices** tab on the [Customer Portal ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/){: new_window}, select **Device List**.
2. Click the instance name where you want to apply the Security Group object.
3. Select **Modify** and mark the Security Group object you want to associate with the instance.

	![Device Menu Instance](./images/device_assign.jpg)

	This figure shows the "allow_icmp" Security Group object being assigned to the private interface of jpmongevsi4 instance.
4. Click **Save** to apply the changes.

5. Reboot the instance.

	**NOTE:** This is a one-time-only step per network interface for instances not created with a security group.

## Next step...
[Edit the Security Group](csg_edit.html) to modify its parameters.  
