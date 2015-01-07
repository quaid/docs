# CentOS

CentOS Linux is a community-supported distribution derived from sources
freely provided to the public by [Red Hat](ftp://ftp.redhat.com/pub/redhat/linux/enterprise/)
for Red Hat Enterprise Linux (RHEL). As such, CentOS Linux aims to be
functionally compatible with RHEL. The CentOS Project mainly changes
packages to remove upstream vendor branding and artwork. CentOS Linux
is no-cost and free to redistribute. Each CentOS version is maintained
for up to 10 years (by means of security updates -- the duration of the
support interval by Red Hat has varied over time with respect to Sources
released). A new CentOS version is released approximately every 2 years
and each CentOS version is periodically updated (roughly every 6 months)
to support newer hardware. This results in a secure, low-maintenance,
reliable, predictable and reproducible Linux environment.


> [wiki.centos.org](https://wiki.centos.org/FrontPage)

%%LOGO%%

# CentOS image documentation

The `centos:latest` tag will always be the most recent version currently
available.

CentOS offers regularly updated images for all active releases. These images
will be updated monthly or as needed for emergency fixes. These rolling
updates are tagged with the major version number only. 
For example: `docker pull centos:6` or `docker pull centos:7`

Additionally, images that correspond to install media are also offered. These
images DO NOT recieve updates as they are intended to match installation iso
contents. If you choose to use these images it is highly recommended that you
include `RUN yum -y update && yum clean all` in your Dockerfile, or otherwise
address any potential security concerns. To use these images, please specify
the minor version tag:

For example `docker pull centos:5.11` or `docker pull centos:6.6`
