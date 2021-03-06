#
# Copyright (c) 2010, 2018 Oracle and/or its affiliates. All rights reserved.
#
# This program and the accompanying materials are made available under the
# terms of the Eclipse Distribution License v. 1.0, which is available at
# http://www.eclipse.org/org/documents/edl-v10.php.
#
# SPDX-License-Identifier: BSD-3-Clause
#

In this sample, issued tokens from an STS are cached ans shared
among two services.

Run the sample:

1. Copy the directory /wsit/wsit/samples/ws-trust/certs/xws-security to 
<GLASSFISH_HOME> or <TOMCAT_HOME>.

2. Edit /wsit/wsit/samples/ws-trust/share/src/fs/build.properties to set java.home and
   tomcat.home/glassfish.home.

3. Edit
   /wsit/wsit/share/ws-trust/share/src/fs/etc/service/PingService.wsdl,
   /wsit/wsit/share/ws-trust/share/src/fs/etc/service1/PingService.wsdl,
   /wsit/wsit/share/ws-trust/share/src/fs/etc/client-config/wsit-client.xml
   and
   /wsit/wsit/samples/ws-trust/share/src/fs/etc/sts/sts.wsdl,
   to replace $WSIT_HOME with your Glassfish/Tomcat location.

4. Start tomcat or glassfish.

5. To run the sample, go to
   /wsit/wsit/samples/ws-trust/share/src/fs, and run "ant run-sample".

6. You will be prompted to enter the username/password. Two pairs alice/alice, bob/bob
   are pre-configured to use with this sample.
