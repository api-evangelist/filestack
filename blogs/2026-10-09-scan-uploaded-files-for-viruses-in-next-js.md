---
title: "Scan Uploaded Files for Viruses in Next.js"
url: "https://blog.filestack.com/scan-uploaded-files-for-viruses-nextjs/"
date: "2026-10-09"
author: "Joshua"
feed_url: "https://blog.filestack.com/feed/"
---
To scan uploaded files for viruses in Next.js, attach a virus_detection workflow to each upload, keep the file pending, verify the signed webhook in a Route Handler, and only redirect to the file once it’s marked clean. Tested on 5 October 2026 with Next.js 16.3.8 and filestack-js 4.3.9. Your users upload files, and other users […] The post Scan Uploaded Files for Viruses in Next.js appeared first on Filestack Blog .
