#!/usr/bin/env python

import liblo, sys, os, subprocess

NSM_URL = os.getenv('NSM_URL')

try: subprocess.check_output(['pgrep','nsmd'])
except subprocess.CalledProcessError: 
    print("[nsm-save] nsmd is not running")
    with open('/tmp/nsmd.log','a') as log:
        log.write("\n[nsm-save] nsmd is not running\n")
    sys.exit()

# send message "/foo/message1" with int, float and string arguments
liblo.send(NSM_URL, "/nsm/server/save")
print("[nsm-save] sent save signal")
with open('/tmp/nsmd.log','a') as log:
    log.write("\n[nsm-save] sent save signal\n")
