# Comparing `tmp/baddns-1.1.784.tar.gz` & `tmp/baddns-1.1.785.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baddns-1.1.784.tar", max compression
+gzip compressed data, was "baddns-1.1.785.tar", max compression
```

## Comparing `baddns-1.1.784.tar` & `baddns-1.1.785.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0    35149 2024-05-09 00:08:14.008420 baddns-1.1.784/LICENSE
--rw-r--r--   0        0        0     3604 2024-05-09 00:08:14.008420 baddns-1.1.784/README.md
--rw-r--r--   0        0        0      687 2024-05-09 00:08:14.008420 baddns-1.1.784/baddns/__init__.py
--rw-r--r--   0        0        0      918 2024-05-09 00:08:14.008420 baddns-1.1.784/baddns/base.py
--rw-r--r--   0        0        0     6304 2024-05-09 00:08:14.008420 baddns-1.1.784/baddns/cli.py
--rw-r--r--   0        0        0        0 2024-05-09 00:08:14.008420 baddns-1.1.784/baddns/lib/__init__.py
--rw-r--r--   0        0        0     5383 2024-05-09 00:08:14.008420 baddns-1.1.784/baddns/lib/dnsmanager.py
--rw-r--r--   0        0        0     8060 2024-05-09 00:08:14.008420 baddns-1.1.784/baddns/lib/dnswalk.py
--rw-r--r--   0        0        0      273 2024-05-09 00:08:14.008420 baddns-1.1.784/baddns/lib/errors.py
--rw-r--r--   0        0        0     2481 2024-05-09 00:08:14.008420 baddns-1.1.784/baddns/lib/findings.py
--rw-r--r--   0        0        0     1886 2024-05-09 00:08:14.008420 baddns-1.1.784/baddns/lib/httpmanager.py
--rw-r--r--   0        0        0     1449 2024-05-09 00:08:14.008420 baddns-1.1.784/baddns/lib/loader.py
--rw-r--r--   0        0        0     1117 2024-05-09 00:08:14.008420 baddns-1.1.784/baddns/lib/logging.py
--rw-r--r--   0        0        0     3362 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/lib/matcher.py
--rw-r--r--   0        0        0     3286 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/lib/signature.py
--rw-r--r--   0        0        0     4100 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/lib/whoismanager.py
--rw-r--r--   0        0        0        0 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/modules/__init__.py
--rw-r--r--   0        0        0     9404 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/modules/cname.py
--rw-r--r--   0        0        0     2129 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/modules/mx.py
--rw-r--r--   0        0        0     4545 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/modules/ns.py
--rw-r--r--   0        0        0     3236 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/modules/nsec.py
--rw-r--r--   0        0        0     6201 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/modules/references.py
--rw-r--r--   0        0        0     4599 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/modules/txt.py
--rw-r--r--   0        0        0     4121 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/modules/zonetransfer.py
--rw-r--r--   0        0        0        0 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/scripts/__init__.py
--rwxr-xr-x   0        0        0    12978 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/scripts/readsources.py
--rwxr-xr-x   0        0        0     4540 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/scripts/signaturetest.py
--rw-r--r--   0        0        0        0 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/.gitignore
--rw-r--r--   0        0        0      341 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/baddns_aws-bucket-website.yml
--rw-r--r--   0        0        0      246 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_000domains.yml
--rw-r--r--   0        0        0      248 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_agilecrm.yml
--rw-r--r--   0        0        0      158 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_aws_ns.yml
--rw-r--r--   0        0        0      242 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_bizland.yml
--rw-r--r--   0        0        0      328 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_brandpad.yml
--rw-r--r--   0        0        0      382 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_brightcove.yml
--rw-r--r--   0        0        0      349 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_campaign_monitor.yml
--rw-r--r--   0        0        0      366 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_cargo_collective.yml
--rw-r--r--   0        0        0      327 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_convertkit.yml
--rw-r--r--   0        0        0      227 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_digitalocean.yml
--rw-r--r--   0        0        0      167 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_dnsmadeeasy.yml
--rw-r--r--   0        0        0      232 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_dnssimple.yml
--rw-r--r--   0        0        0      184 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_domain.yml
--rw-r--r--   0        0        0      239 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_dotster.yml
--rw-r--r--   0        0        0     1331 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_elastic_beanstalk.yml
--rw-r--r--   0        0        0      307 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_frontify.yml
--rw-r--r--   0        0        0      297 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_getresponse.yml
--rw-r--r--   0        0        0      475 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_github_pages.yml
--rw-r--r--   0        0        0      170 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_googlecloud.yml
--rw-r--r--   0        0        0      306 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_hatenablog.yml
--rw-r--r--   0        0        0      300 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_helpscout.yml
--rw-r--r--   0        0        0      193 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_hostinger.yml
--rw-r--r--   0        0        0      217 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_hurricane_electric.yml
--rw-r--r--   0        0        0      309 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_jetbrains.yml
--rw-r--r--   0        0        0      248 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_launchrock_cname.yml
--rw-r--r--   0        0        0      184 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_linode.yml
--rw-r--r--   0        0        0      298 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_mashery.yml
--rw-r--r--   0        0        0      199 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_mediatemplate.yml
--rw-r--r--   0        0        0      319 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_mysmartjobboard.yml
--rw-r--r--   0        0        0      158 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_name.yml
--rw-r--r--   0        0        0      300 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_netlify.yml
--rw-r--r--   0        0        0      401 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_ngrok.yml
--rw-r--r--   0        0        0      158 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_nsone.yml
--rw-r--r--   0        0        0      172 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_reg.yml
--rw-r--r--   0        0        0      303 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_shopify.yml
--rw-r--r--   0        0        0      352 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_simplebooklet.yml
--rw-r--r--   0        0        0      330 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_smartjobboard.yml
--rw-r--r--   0        0        0      290 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_surge.yml
--rw-r--r--   0        0        0      315 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_surveysparrow.yml
--rw-r--r--   0        0        0      323 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_teamwork.yml
--rw-r--r--   0        0        0      344 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_thinkific.yml
--rw-r--r--   0        0        0      200 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_tierranet.yml
--rw-r--r--   0        0        0      351 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_tribe.yml
--rw-r--r--   0        0        0      298 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_tumblr.yml
--rw-r--r--   0        0        0      338 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_vendhq.yml
--rw-r--r--   0        0        0      353 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_webflow.yml
--rw-r--r--   0        0        0      323 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_wishpond.yml
--rw-r--r--   0        0        0      306 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_wordpress_com_cname.yml
--rw-r--r--   0        0        0      215 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_wordpress_com_ns.yml
--rw-r--r--   0        0        0      359 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_zohoforms.yml
--rw-r--r--   0        0        0      324 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/dnsreaper_zohoforms_in.yml
--rw-r--r--   0        0        0      411 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_aftership-takeover.yml
--rw-r--r--   0        0        0      347 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_agilecrm-takeover.yml
--rw-r--r--   0        0        0      366 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_aha-takeover.yml
--rw-r--r--   0        0        0      511 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_airee-takeover.yml
--rw-r--r--   0        0        0      382 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_anima-takeover.yml
--rw-r--r--   0        0        0      366 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_announcekit-takeover.yml
--rw-r--r--   0        0        0      479 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_aws-bucket-takeover.yml
--rw-r--r--   0        0        0     1022 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_azure-takeover-detection.yml
--rw-r--r--   0        0        0      456 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_bigcartel-takeover.yml
--rw-r--r--   0        0        0      407 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_bitbucket-takeover.yml
--rw-r--r--   0        0        0      406 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_campaignmonitor-takeover.yml
--rw-r--r--   0        0        0      382 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_canny-takeover.yml
--rw-r--r--   0        0        0      415 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_clever-takeover.yml
--rw-r--r--   0        0        0      374 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_flexbe-takeover.yml
--rw-r--r--   0        0        0      529 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_flywheel-takeover.yml
--rw-r--r--   0        0        0      343 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_gemfury-takeover.yml
--rw-r--r--   0        0        0      356 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_ghost-takeover.yml
--rw-r--r--   0        0        0      368 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_gitbook-takeover.yml
--rw-r--r--   0        0        0      430 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_gohire-takeover.yml
--rw-r--r--   0        0        0      365 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_helpdocs-takeover.yml
--rw-r--r--   0        0        0      387 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_helpjuice-takeover.yml
--rw-r--r--   0        0        0      394 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_helprace-takeover.yml
--rw-r--r--   0        0        0      487 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_heroku-takeover.yml
--rw-r--r--   0        0        0      357 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_hubspot-takeover.yml
--rw-r--r--   0        0        0      422 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_intercom-takeover.yml
--rw-r--r--   0        0        0      410 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_launchrock-takeover.yml
--rw-r--r--   0        0        0      482 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_leadpages-takeover.yml
--rw-r--r--   0        0        0      359 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_lemlist-takeover.yml
--rw-r--r--   0        0        0      320 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_meteor-takeover.yml
--rw-r--r--   0        0        0      379 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_pagewiz-takeover.yml
--rw-r--r--   0        0        0      346 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_pantheon-takeover.yml
--rw-r--r--   0        0        0      398 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_pingdom-takeover.yml
--rw-r--r--   0        0        0      394 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_proposify-takeover.yml
--rw-r--r--   0        0        0      336 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_readme-takeover.yml
--rw-r--r--   0        0        0      336 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_readthedocs-takeover.yml
--rw-r--r--   0        0        0      788 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_shopify-takeover.yml
--rw-r--r--   0        0        0      365 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_simplebooklet-takeover.yml
--rw-r--r--   0        0        0      332 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_smugmug-takeover.yml
--rw-r--r--   0        0        0      424 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_softr-takeover.yml
--rw-r--r--   0        0        0      623 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_sprintful-takeover.yml
--rw-r--r--   0        0        0      462 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_squadcast-takeover.yml
--rw-r--r--   0        0        0      394 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_strikingly-takeover.yml
--rw-r--r--   0        0        0      508 2024-05-09 00:08:14.012420 baddns-1.1.784/baddns/signatures/nucleitemplates_tilda-takeover.yml
--rw-r--r--   0        0        0      370 2024-05-09 00:08:14.016420 baddns-1.1.784/baddns/signatures/nucleitemplates_uberflip-takeover.yml
--rw-r--r--   0        0        0      434 2024-05-09 00:08:14.016420 baddns-1.1.784/baddns/signatures/nucleitemplates_uptime-takeover.yml
--rw-r--r--   0        0        0      356 2024-05-09 00:08:14.016420 baddns-1.1.784/baddns/signatures/nucleitemplates_uservoice-takeover.yml
--rw-r--r--   0        0        0      354 2024-05-09 00:08:14.016420 baddns-1.1.784/baddns/signatures/nucleitemplates_vend-takeover.yml
--rw-r--r--   0        0        0      348 2024-05-09 00:08:14.016420 baddns-1.1.784/baddns/signatures/nucleitemplates_vercel-takeover.yml
--rw-r--r--   0        0        0      423 2024-05-09 00:08:14.016420 baddns-1.1.784/baddns/signatures/nucleitemplates_wishpond-takeover.yml
--rw-r--r--   0        0        0      390 2024-05-09 00:08:14.016420 baddns-1.1.784/baddns/signatures/nucleitemplates_wix-takeover.yml
--rw-r--r--   0        0        0      359 2024-05-09 00:08:14.016420 baddns-1.1.784/baddns/signatures/nucleitemplates_wufoo-takeover.yml
--rw-r--r--   0        0        0      363 2024-05-09 00:08:14.016420 baddns-1.1.784/baddns/signatures/nucleitemplates_zendesk-takeover.yml
--rw-r--r--   0        0        0    10568 2024-05-09 00:08:14.016420 baddns-1.1.784/baddns/signatures/signature_history.txt
--rw-r--r--   0        0        0     1436 2024-05-09 00:08:28.064313 baddns-1.1.784/pyproject.toml
--rw-r--r--   0        0        0     4749 1970-01-01 00:00:00.000000 baddns-1.1.784/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-15 19:18:06.124731 baddns-1.1.785/LICENSE
+-rw-r--r--   0        0        0     3720 2024-05-15 19:18:06.124731 baddns-1.1.785/README.md
+-rw-r--r--   0        0        0      687 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/__init__.py
+-rw-r--r--   0        0        0      918 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/base.py
+-rw-r--r--   0        0        0     6304 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/cli.py
+-rw-r--r--   0        0        0        0 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/__init__.py
+-rw-r--r--   0        0        0     5383 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/dnsmanager.py
+-rw-r--r--   0        0        0     8060 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/dnswalk.py
+-rw-r--r--   0        0        0      273 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/errors.py
+-rw-r--r--   0        0        0     2481 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/findings.py
+-rw-r--r--   0        0        0     1886 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/httpmanager.py
+-rw-r--r--   0        0        0     1449 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/loader.py
+-rw-r--r--   0        0        0     1117 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/logging.py
+-rw-r--r--   0        0        0     3362 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/matcher.py
+-rw-r--r--   0        0        0     3286 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/signature.py
+-rw-r--r--   0        0        0     4100 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/lib/whoismanager.py
+-rw-r--r--   0        0        0        0 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/modules/__init__.py
+-rw-r--r--   0        0        0     9404 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/modules/cname.py
+-rw-r--r--   0        0        0     2129 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/modules/mx.py
+-rw-r--r--   0        0        0     4545 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/modules/ns.py
+-rw-r--r--   0        0        0     3236 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/modules/nsec.py
+-rw-r--r--   0        0        0     6201 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/modules/references.py
+-rw-r--r--   0        0        0     4599 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/modules/txt.py
+-rw-r--r--   0        0        0     4121 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/modules/zonetransfer.py
+-rw-r--r--   0        0        0        0 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/scripts/__init__.py
+-rwxr-xr-x   0        0        0    12978 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/scripts/readsources.py
+-rwxr-xr-x   0        0        0     4540 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/scripts/signaturetest.py
+-rw-r--r--   0        0        0        0 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/.gitignore
+-rw-r--r--   0        0        0      341 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/baddns_aws-bucket-website.yml
+-rw-r--r--   0        0        0      246 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_000domains.yml
+-rw-r--r--   0        0        0      248 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_agilecrm.yml
+-rw-r--r--   0        0        0      158 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_aws_ns.yml
+-rw-r--r--   0        0        0      242 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_bizland.yml
+-rw-r--r--   0        0        0      328 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_brandpad.yml
+-rw-r--r--   0        0        0      382 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_brightcove.yml
+-rw-r--r--   0        0        0      349 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_campaign_monitor.yml
+-rw-r--r--   0        0        0      366 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_cargo_collective.yml
+-rw-r--r--   0        0        0      327 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_convertkit.yml
+-rw-r--r--   0        0        0      227 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_digitalocean.yml
+-rw-r--r--   0        0        0      167 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_dnsmadeeasy.yml
+-rw-r--r--   0        0        0      232 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_dnssimple.yml
+-rw-r--r--   0        0        0      184 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_domain.yml
+-rw-r--r--   0        0        0      239 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_dotster.yml
+-rw-r--r--   0        0        0     1331 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_elastic_beanstalk.yml
+-rw-r--r--   0        0        0      307 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_frontify.yml
+-rw-r--r--   0        0        0      297 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_getresponse.yml
+-rw-r--r--   0        0        0      475 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_github_pages.yml
+-rw-r--r--   0        0        0      170 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_googlecloud.yml
+-rw-r--r--   0        0        0      306 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_hatenablog.yml
+-rw-r--r--   0        0        0      300 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_helpscout.yml
+-rw-r--r--   0        0        0      193 2024-05-15 19:18:06.124731 baddns-1.1.785/baddns/signatures/dnsreaper_hostinger.yml
+-rw-r--r--   0        0        0      217 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_hurricane_electric.yml
+-rw-r--r--   0        0        0      309 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_jetbrains.yml
+-rw-r--r--   0        0        0      248 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_launchrock_cname.yml
+-rw-r--r--   0        0        0      184 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_linode.yml
+-rw-r--r--   0        0        0      298 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_mashery.yml
+-rw-r--r--   0        0        0      199 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_mediatemplate.yml
+-rw-r--r--   0        0        0      319 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_mysmartjobboard.yml
+-rw-r--r--   0        0        0      158 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_name.yml
+-rw-r--r--   0        0        0      300 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_netlify.yml
+-rw-r--r--   0        0        0      401 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_ngrok.yml
+-rw-r--r--   0        0        0      158 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_nsone.yml
+-rw-r--r--   0        0        0      172 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_reg.yml
+-rw-r--r--   0        0        0      303 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_shopify.yml
+-rw-r--r--   0        0        0      352 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_simplebooklet.yml
+-rw-r--r--   0        0        0      330 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_smartjobboard.yml
+-rw-r--r--   0        0        0      290 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_surge.yml
+-rw-r--r--   0        0        0      315 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_surveysparrow.yml
+-rw-r--r--   0        0        0      323 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_teamwork.yml
+-rw-r--r--   0        0        0      344 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_thinkific.yml
+-rw-r--r--   0        0        0      200 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_tierranet.yml
+-rw-r--r--   0        0        0      351 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_tribe.yml
+-rw-r--r--   0        0        0      298 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_tumblr.yml
+-rw-r--r--   0        0        0      338 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_vendhq.yml
+-rw-r--r--   0        0        0      353 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_webflow.yml
+-rw-r--r--   0        0        0      323 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_wishpond.yml
+-rw-r--r--   0        0        0      306 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_wordpress_com_cname.yml
+-rw-r--r--   0        0        0      215 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_wordpress_com_ns.yml
+-rw-r--r--   0        0        0      359 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_zohoforms.yml
+-rw-r--r--   0        0        0      324 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/dnsreaper_zohoforms_in.yml
+-rw-r--r--   0        0        0      411 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_aftership-takeover.yml
+-rw-r--r--   0        0        0      347 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_agilecrm-takeover.yml
+-rw-r--r--   0        0        0      366 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_aha-takeover.yml
+-rw-r--r--   0        0        0      511 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_airee-takeover.yml
+-rw-r--r--   0        0        0      382 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_anima-takeover.yml
+-rw-r--r--   0        0        0      366 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_announcekit-takeover.yml
+-rw-r--r--   0        0        0      479 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_aws-bucket-takeover.yml
+-rw-r--r--   0        0        0     1022 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_azure-takeover-detection.yml
+-rw-r--r--   0        0        0      456 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_bigcartel-takeover.yml
+-rw-r--r--   0        0        0      407 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_bitbucket-takeover.yml
+-rw-r--r--   0        0        0      406 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_campaignmonitor-takeover.yml
+-rw-r--r--   0        0        0      382 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_canny-takeover.yml
+-rw-r--r--   0        0        0      415 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_clever-takeover.yml
+-rw-r--r--   0        0        0      374 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_flexbe-takeover.yml
+-rw-r--r--   0        0        0      529 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_flywheel-takeover.yml
+-rw-r--r--   0        0        0      343 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_gemfury-takeover.yml
+-rw-r--r--   0        0        0      356 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_ghost-takeover.yml
+-rw-r--r--   0        0        0      368 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_gitbook-takeover.yml
+-rw-r--r--   0        0        0      430 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_gohire-takeover.yml
+-rw-r--r--   0        0        0      365 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_helpdocs-takeover.yml
+-rw-r--r--   0        0        0      387 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_helpjuice-takeover.yml
+-rw-r--r--   0        0        0      394 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_helprace-takeover.yml
+-rw-r--r--   0        0        0      487 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_heroku-takeover.yml
+-rw-r--r--   0        0        0      357 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_hubspot-takeover.yml
+-rw-r--r--   0        0        0      422 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_intercom-takeover.yml
+-rw-r--r--   0        0        0      410 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_launchrock-takeover.yml
+-rw-r--r--   0        0        0      482 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_leadpages-takeover.yml
+-rw-r--r--   0        0        0      359 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_lemlist-takeover.yml
+-rw-r--r--   0        0        0      320 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_meteor-takeover.yml
+-rw-r--r--   0        0        0      379 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_pagewiz-takeover.yml
+-rw-r--r--   0        0        0      346 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_pantheon-takeover.yml
+-rw-r--r--   0        0        0      398 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_pingdom-takeover.yml
+-rw-r--r--   0        0        0      394 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_proposify-takeover.yml
+-rw-r--r--   0        0        0      336 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_readme-takeover.yml
+-rw-r--r--   0        0        0      336 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_readthedocs-takeover.yml
+-rw-r--r--   0        0        0      788 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_shopify-takeover.yml
+-rw-r--r--   0        0        0      365 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_simplebooklet-takeover.yml
+-rw-r--r--   0        0        0      332 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_smugmug-takeover.yml
+-rw-r--r--   0        0        0      424 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_softr-takeover.yml
+-rw-r--r--   0        0        0      623 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_sprintful-takeover.yml
+-rw-r--r--   0        0        0      462 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_squadcast-takeover.yml
+-rw-r--r--   0        0        0      394 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_strikingly-takeover.yml
+-rw-r--r--   0        0        0      508 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_tilda-takeover.yml
+-rw-r--r--   0        0        0      370 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_uberflip-takeover.yml
+-rw-r--r--   0        0        0      434 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_uptime-takeover.yml
+-rw-r--r--   0        0        0      356 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_uservoice-takeover.yml
+-rw-r--r--   0        0        0      354 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_vend-takeover.yml
+-rw-r--r--   0        0        0      348 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_vercel-takeover.yml
+-rw-r--r--   0        0        0      423 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_wishpond-takeover.yml
+-rw-r--r--   0        0        0      390 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_wix-takeover.yml
+-rw-r--r--   0        0        0      359 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_wufoo-takeover.yml
+-rw-r--r--   0        0        0      363 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/nucleitemplates_zendesk-takeover.yml
+-rw-r--r--   0        0        0    10568 2024-05-15 19:18:06.128731 baddns-1.1.785/baddns/signatures/signature_history.txt
+-rw-r--r--   0        0        0     1436 2024-05-15 19:18:21.532751 baddns-1.1.785/pyproject.toml
+-rw-r--r--   0        0        0     4865 1970-01-01 00:00:00.000000 baddns-1.1.785/PKG-INFO
```

### Comparing `baddns-1.1.784/LICENSE` & `baddns-1.1.785/LICENSE`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/README.md` & `baddns-1.1.785/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 [![codecov](https://codecov.io/gh/blacklanternsecurity/baddns/branch/main/graph/badge.svg)](https://codecov.io/gh/blacklanternsecurity/baddns)
 [![Pypi Downloads](https://img.shields.io/pypi/dm/baddns)](https://pypi.org/project/baddns)
 
 <p align="left"><img width="300" height="300" src="https://github.com/blacklanternsecurity/baddns/assets/24899338/2ca1fe25-e834-4df8-8b02-8bf8f60f6e31"></p>
 
 BadDNS is a standalone tool and [BBOT](https://github.com/blacklanternsecurity/bbot) module for detecting domain/subdomain takeovers of all kinds, including other DNS issues like NSEC walks and Subdomain Takeovers. 
 
+Check out the [introductory blog](https://blog.blacklanternsecurity.com/p/introducing-baddns) on the BLS substack!
+
 ## Installation
 
 We have a [pypi](https://pypi.org/project/baddns/) package, so you can just do `pip install baddns` to make use of the library.
 
 ## Usage 
 
 After installing with pip, you can just run `baddns` from the command line.
```

### Comparing `baddns-1.1.784/baddns/__init__.py` & `baddns-1.1.785/baddns/__init__.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/base.py` & `baddns-1.1.785/baddns/base.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/cli.py` & `baddns-1.1.785/baddns/cli.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/lib/dnsmanager.py` & `baddns-1.1.785/baddns/lib/dnsmanager.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/lib/dnswalk.py` & `baddns-1.1.785/baddns/lib/dnswalk.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/lib/findings.py` & `baddns-1.1.785/baddns/lib/findings.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/lib/httpmanager.py` & `baddns-1.1.785/baddns/lib/httpmanager.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/lib/loader.py` & `baddns-1.1.785/baddns/lib/loader.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/lib/logging.py` & `baddns-1.1.785/baddns/lib/logging.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/lib/matcher.py` & `baddns-1.1.785/baddns/lib/matcher.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/lib/signature.py` & `baddns-1.1.785/baddns/lib/signature.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/lib/whoismanager.py` & `baddns-1.1.785/baddns/lib/whoismanager.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/modules/cname.py` & `baddns-1.1.785/baddns/modules/cname.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/modules/mx.py` & `baddns-1.1.785/baddns/modules/mx.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/modules/ns.py` & `baddns-1.1.785/baddns/modules/ns.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/modules/nsec.py` & `baddns-1.1.785/baddns/modules/nsec.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/modules/references.py` & `baddns-1.1.785/baddns/modules/references.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/modules/txt.py` & `baddns-1.1.785/baddns/modules/txt.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/modules/zonetransfer.py` & `baddns-1.1.785/baddns/modules/zonetransfer.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/scripts/readsources.py` & `baddns-1.1.785/baddns/scripts/readsources.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/scripts/signaturetest.py` & `baddns-1.1.785/baddns/scripts/signaturetest.py`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/signatures/dnsreaper_elastic_beanstalk.yml` & `baddns-1.1.785/baddns/signatures/dnsreaper_elastic_beanstalk.yml`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/signatures/nucleitemplates_azure-takeover-detection.yml` & `baddns-1.1.785/baddns/signatures/nucleitemplates_azure-takeover-detection.yml`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/signatures/nucleitemplates_flywheel-takeover.yml` & `baddns-1.1.785/baddns/signatures/nucleitemplates_flywheel-takeover.yml`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/signatures/nucleitemplates_shopify-takeover.yml` & `baddns-1.1.785/baddns/signatures/nucleitemplates_shopify-takeover.yml`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/signatures/nucleitemplates_sprintful-takeover.yml` & `baddns-1.1.785/baddns/signatures/nucleitemplates_sprintful-takeover.yml`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/baddns/signatures/signature_history.txt` & `baddns-1.1.785/baddns/signatures/signature_history.txt`

 * *Files identical despite different names*

### Comparing `baddns-1.1.784/pyproject.toml` & `baddns-1.1.785/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "baddns"
-version = "v1.1.784"
+version = "v1.1.785"
 description = "Check subdomains for subdomain takeovers and other DNS tomfoolery"
 authors = ["liquidsec <paul.mueller08@gmail.com>"]
 repository = "https://github.com/blacklanternsecurity/baddns"
 homepage = "https://github.com/blacklanternsecurity/baddns"
 documentation = "https://www.blacklanternsecurity.com/baddns/"
 license = "GPL-3.0"
 readme = "README.md"
```

### Comparing `baddns-1.1.784/PKG-INFO` & `baddns-1.1.785/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baddns
-Version: 1.1.784
+Version: 1.1.785
 Summary: Check subdomains for subdomain takeovers and other DNS tomfoolery
 Home-page: https://github.com/blacklanternsecurity/baddns
 License: GPL-3.0
 Author: liquidsec
 Author-email: paul.mueller08@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -34,14 +34,16 @@
 [![codecov](https://codecov.io/gh/blacklanternsecurity/baddns/branch/main/graph/badge.svg)](https://codecov.io/gh/blacklanternsecurity/baddns)
 [![Pypi Downloads](https://img.shields.io/pypi/dm/baddns)](https://pypi.org/project/baddns)
 
 <p align="left"><img width="300" height="300" src="https://github.com/blacklanternsecurity/baddns/assets/24899338/2ca1fe25-e834-4df8-8b02-8bf8f60f6e31"></p>
 
 BadDNS is a standalone tool and [BBOT](https://github.com/blacklanternsecurity/bbot) module for detecting domain/subdomain takeovers of all kinds, including other DNS issues like NSEC walks and Subdomain Takeovers. 
 
+Check out the [introductory blog](https://blog.blacklanternsecurity.com/p/introducing-baddns) on the BLS substack!
+
 ## Installation
 
 We have a [pypi](https://pypi.org/project/baddns/) package, so you can just do `pip install baddns` to make use of the library.
 
 ## Usage 
 
 After installing with pip, you can just run `baddns` from the command line.
```

