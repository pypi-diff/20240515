# Comparing `tmp/neon-skill-weather-2.0.1a1.tar.gz` & `tmp/neon-skill-weather-2.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-weather-2.0.1a1.tar", last modified: Tue May 14 01:06:51 2024, max compression
+gzip compressed data, was "neon-skill-weather-2.0.1a2.tar", last modified: Wed May 15 19:16:38 2024, max compression
```

## Comparing `neon-skill-weather-2.0.1a1.tar` & `neon-skill-weather-2.0.1a2.tar`

### file list

```diff
@@ -1,1550 +1,1550 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.722939 neon-skill-weather-2.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-14 01:06:51.722939 neon-skill-weather-2.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    48627 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.546939 neon-skill-weather-2.0.1a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.534939 neon-skill-weather-2.0.1a1/locale/ca-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.550939 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/and.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.550939 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/condition/clear sky.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.554939 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/current/current-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.554939 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/daily-wind-light-loaction.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.558939 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.558939 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/error/location-not-found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/error/no-forecast.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.558939 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.558939 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.558939 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/weekly/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/dialog/weekly/weekly-temperature.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.558939 neon-skill-weather-2.0.1a1/locale/ca-es/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.558939 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.562939 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/condition/do.i.need.an.umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.562939 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.562939 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.562939 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.562939 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ca-es/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.534939 neon-skill-weather-2.0.1a1/locale/da-dk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.566939 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/and.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.566939 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/condition/clear sky.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.566939 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.570939 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.570939 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.570939 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/error/location-not-found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/error/no-forecast.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.574939 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.574939 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.574939 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/weekly/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/dialog/weekly/weekly-temperature.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.574939 neon-skill-weather-2.0.1a1/locale/da-dk/regex/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.574939 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.574939 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/condition/do-i-need-an-umbrella-intent
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.578939 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.578939 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.578939 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.578939 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/da-dk/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.534939 neon-skill-weather-2.0.1a1/locale/de-de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.578939 neon-skill-weather-2.0.1a1/locale/de-de/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/and.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.578939 neon-skill-weather-2.0.1a1/locale/de-de/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/condition/clear sky.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.586939 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-humidity-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-sunrise-future-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-sunrise-future-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-sunrise-past-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-sunrise-past-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-sunset-future-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-sunset-future-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-sunset-past-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-sunset-past-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/current/current-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.590939 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-humidity-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-precipitation-next-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-precipitation-next-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-precipitation-next-none-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-precipitation-next-none-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-sunrise-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-sunrise-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-sunset-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-sunset-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.590939 neon-skill-weather-2.0.1a1/locale/de-de/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.590939 neon-skill-weather-2.0.1a1/locale/de-de/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/error/location-not-found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/error/no-forecast.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.590939 neon-skill-weather-2.0.1a1/locale/de-de/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/hourly/hourly-precipitation-next-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/hourly/hourly-precipitation-next-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.590939 neon-skill-weather-2.0.1a1/locale/de-de/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.594939 neon-skill-weather-2.0.1a1/locale/de-de/dialog/weekly/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/weekly/weekly-condition.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/dialog/weekly/weekly-temperature.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.594939 neon-skill-weather-2.0.1a1/locale/de-de/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.594939 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.594939 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/condition/do.i.need.an.umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.594939 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.598939 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.598939 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.598939 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/de-de/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.538939 neon-skill-weather-2.0.1a1/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.598939 neon-skill-weather-2.0.1a1/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/and.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.598939 neon-skill-weather-2.0.1a1/locale/en-us/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/condition/clear-sky.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/condition/clouds.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/condition/humidity.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.602939 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-humidity-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-sunrise-future-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-sunrise-future-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-sunrise-past-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-sunrise-past-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-sunset-future-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-sunset-future-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-sunset-past-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-sunset-past-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/current-wind-strong-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/current/currrent-clouds-alternative-local.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.606939 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-humidity-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-precipitation-next-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-precipitation-next-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-precipitation-next-none-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-precipitation-next-none-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-sunrise-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-sunrise-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-sunset-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-sunset-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.610939 neon-skill-weather-2.0.1a1/locale/en-us/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.610939 neon-skill-weather-2.0.1a1/locale/en-us/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/error/forty-eight-hours-available.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/error/location-not-found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/error/no-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/error/seven-days-available.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.610939 neon-skill-weather-2.0.1a1/locale/en-us/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/hourly/hourly-precipitation-next-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/hourly/hourly-precipitation-next-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/hourly/hourly-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.610939 neon-skill-weather-2.0.1a1/locale/en-us/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.610939 neon-skill-weather-2.0.1a1/locale/en-us/dialog/weekly/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/weekly/weekly-condition.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/dialog/weekly/weekly-temperature.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.610939 neon-skill-weather-2.0.1a1/locale/en-us/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.614939 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.614939 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/condition/do-i-need-an-umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.614939 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/date-time/few.voc
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/date-time/number-days.voc
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/like.voc
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/location.voc
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/outside.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.618939 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.618939 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.618939 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/en-us/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.538939 neon-skill-weather-2.0.1a1/locale/es-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.618939 neon-skill-weather-2.0.1a1/locale/es-es/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.618939 neon-skill-weather-2.0.1a1/locale/es-es/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/condition/humidity.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/condition/snow.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.618939 neon-skill-weather-2.0.1a1/locale/es-es/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/current/current-weather-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.618939 neon-skill-weather-2.0.1a1/locale/es-es/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/daily/daily-weather-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.622939 neon-skill-weather-2.0.1a1/locale/es-es/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.622939 neon-skill-weather-2.0.1a1/locale/es-es/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/error/location-not-found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.622939 neon-skill-weather-2.0.1a1/locale/es-es/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.622939 neon-skill-weather-2.0.1a1/locale/es-es/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.622939 neon-skill-weather-2.0.1a1/locale/es-es/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.622939 neon-skill-weather-2.0.1a1/locale/es-es/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.622939 neon-skill-weather-2.0.1a1/locale/es-es/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.622939 neon-skill-weather-2.0.1a1/locale/es-es/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.622939 neon-skill-weather-2.0.1a1/locale/es-es/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/vocabulary/sunset.voc
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/es-es/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.538939 neon-skill-weather-2.0.1a1/locale/eu-eu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.622939 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.626939 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/condition/clear-sky.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/condition/clouds.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/condition/humidity.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.630939 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-humidity-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-sunrise-future-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-sunrise-future-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-sunrise-past-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-sunrise-past-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-sunset-future-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-sunset-future-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-sunset-past-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-sunset-past-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/current-wind-strong-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/current/currrent-clouds-alternative-local.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.634939 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-humidity-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-precipitation-next-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-precipitation-next-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-precipitation-next-none-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-precipitation-next-none-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-sunrise-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-sunrise-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-sunset-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-sunset-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.634939 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.634939 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/error/forty-eight-hours-available.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/error/location-not-found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/error/no-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/error/seven-days-available.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.634939 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/hourly/hourly-precipitation-next-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/hourly/hourly-precipitation-next-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/hourly/hourly-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.638939 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.638939 neon-skill-weather-2.0.1a1/locale/eu-eu/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.638939 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.638939 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/condition/do-i-need-an-umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.642939 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/date-time/few.voc
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/date-time/number-days.voc
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.642939 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.642939 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.642939 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.542940 neon-skill-weather-2.0.1a1/locale/fr-fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.642939 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.642939 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/condition/snow.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.642939 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/current/current-weather-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.642939 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/daily/daily-weather-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.646939 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.646939 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/error/location-not-found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.646939 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.646939 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.646939 neon-skill-weather-2.0.1a1/locale/fr-fr/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.646939 neon-skill-weather-2.0.1a1/locale/fr-fr/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.646939 neon-skill-weather-2.0.1a1/locale/fr-fr/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.646939 neon-skill-weather-2.0.1a1/locale/fr-fr/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.646939 neon-skill-weather-2.0.1a1/locale/fr-fr/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/vocabulary/sunset.voc
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/fr-fr/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.542940 neon-skill-weather-2.0.1a1/locale/gl-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.646939 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/and.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.650939 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/condition/clear sky.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/condition/percentage-number.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.650939 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/current/current-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.654939 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.654939 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.654939 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/error/location-not-found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/error/no-forecast.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.658939 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/hourly/hourly-condition-expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.658939 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.658939 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/weekly/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/dialog/weekly/weekly-temperature.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.658939 neon-skill-weather-2.0.1a1/locale/gl-es/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.658939 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.658939 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/condition/do.i.need.an.umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.662939 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.662939 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.662939 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.662939 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/gl-es/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.542940 neon-skill-weather-2.0.1a1/locale/it-it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.662939 neon-skill-weather-2.0.1a1/locale/it-it/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.662939 neon-skill-weather-2.0.1a1/locale/it-it/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/condition/snow.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.666939 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/current/current-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.666939 neon-skill-weather-2.0.1a1/locale/it-it/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.666939 neon-skill-weather-2.0.1a1/locale/it-it/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.666939 neon-skill-weather-2.0.1a1/locale/it-it/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/error/location-not-found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.666939 neon-skill-weather-2.0.1a1/locale/it-it/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.666939 neon-skill-weather-2.0.1a1/locale/it-it/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.666939 neon-skill-weather-2.0.1a1/locale/it-it/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.666939 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.670939 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/condition/do.i.need.an.umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.670939 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.670939 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.670939 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.670939 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/it-it/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.546939 neon-skill-weather-2.0.1a1/locale/nl-nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.670939 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.670939 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/condition/snow.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.670939 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/current/current-weather-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.670939 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/daily/daily-weather-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.670939 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/direction/southwest.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.670939 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/error/location-not-found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.670939 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.674939 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.674939 neon-skill-weather-2.0.1a1/locale/nl-nl/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.674939 neon-skill-weather-2.0.1a1/locale/nl-nl/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.674939 neon-skill-weather-2.0.1a1/locale/nl-nl/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.674939 neon-skill-weather-2.0.1a1/locale/nl-nl/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.674939 neon-skill-weather-2.0.1a1/locale/nl-nl/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/vocabulary/sunset.voc
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/nl-nl/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.546939 neon-skill-weather-2.0.1a1/locale/pt-br/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.674939 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/and.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.674939 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/condition/clear sky.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.678939 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/current/current-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.678939 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/daily/daily-temperature-high.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.678939 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.678939 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/error/location-not-found.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.678939 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.682939 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.682939 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/weekly/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/dialog/weekly/weekly-temperature.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.682939 neon-skill-weather-2.0.1a1/locale/pt-br/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.682939 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.682939 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/condition/do.i.need.an.umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.682939 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.686939 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.686939 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.686939 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/pt-br/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.546939 neon-skill-weather-2.0.1a1/locale/ru-ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.686939 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/and.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.686939 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/condition/clear-sky.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/condition/clouds.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/condition/humidity.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.690939 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-humidity-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-sunrise-future-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-sunrise-future-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-sunrise-past-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-sunrise-past-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-sunset-future-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-sunset-future-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-sunset-past-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-sunset-past-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-wind-strong-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/currrent-clouds-alternative-local.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.694939 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-humidity-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-precipitation-next-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-precipitation-next-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-precipitation-next-none-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-precipitation-next-none-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-sunrise-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-sunrise-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-sunset-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-sunset-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-weather-loation.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.694939 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.694939 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/error/forty-eight-hours-available.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/error/location-not-found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/error/no-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/error/seven-days-available.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.694939 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/hourly/hourly-precipitation-next-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/hourly/hourly-precipitation-next-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/hourly/hourly-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.694939 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.698939 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/weekly/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/weekly/weekly-condition.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/weekly/weekly-temperature.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.698939 neon-skill-weather-2.0.1a1/locale/ru-ru/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.698939 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.698939 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/condition/do-i-need-an-umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/condition/fog.voc
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.698939 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/date-time/few.voc
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/date-time/number-days.voc
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/like.voc
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/location.voc
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/outside.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.698939 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.702939 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.702939 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.550939 neon-skill-weather-2.0.1a1/locale/sv-se/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.702939 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/and.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.702939 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/condition/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/condition/clear sky.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/condition/clear.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/condition/no precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/condition/precipitation expected.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/condition/rain.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/condition/snow.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/condition/thunderstorm.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.702939 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-humidity-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-temperature-high-low.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/current/current-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.706939 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/daily-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/daily-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/daily-temperature-high-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/daily-temperature-high-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/daily-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/daily-temperature-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/daily-temperature-low-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/daily-temperature-low-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/daily-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/daily-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/daily-wind-light-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/daily-wind-light-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/daily-wind-moderate-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/daily-wind-moderate-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/daily-wind-strong-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/daily-wind-strong-location.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.706939 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/direction/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/direction/east.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/direction/north.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/direction/northeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/direction/northwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/direction/south.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/direction/southeast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/direction/southwest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/direction/west.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.706939 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/error/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/error/cant-get-forecast.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/error/location-not-found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/error/no-forecast.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.710939 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/hourly/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/hourly/hourly-condition-alternative-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/hourly/hourly-condition-alternative-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/hourly/hourly-condition-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/hourly/hourly-condition-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/hourly/hourly-condition-not-expected-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/hourly/hourly-condition-not-expected-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/hourly/hourly-temperature-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/hourly/hourly-weather-local.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/hourly/hourly-weather-location.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/percentage-number.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.710939 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/unit/celsius.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/unit/fahrenheit.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/unit/meters per second.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/unit/miles per hour.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.710939 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/weekly/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/dialog/weekly/weekly-temperature.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.710939 neon-skill-weather-2.0.1a1/locale/sv-se/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/regex/location.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.710939 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.710939 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/condition/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/condition/clear.voc
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/condition/clouds.voc
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/condition/do.i.need.an.umbrella.intent
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/condition/humidity.voc
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/condition/precipitation.voc
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/condition/rain.voc
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/condition/snow.voc
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/condition/thunderstorm.voc
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/condition/windy.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.710939 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/date-time/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/date-time/couple.voc
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/date-time/later.voc
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/date-time/next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/date-time/now.voc
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/date-time/relative-day.voc
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/date-time/relative-time.voc
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/date-time/today.voc
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/date-time/week.voc
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/date-time/weekend.voc
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/forecast.voc
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/location.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.714939 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/query/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/query/confirm-query-current.voc
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/query/confirm-query-future.voc
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/query/confirm-query.voc
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/query/how.voc
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/query/query.voc
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/query/when.voc
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/sunrise.voc
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/sunset.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.714939 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/temperature/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/temperature/cold.voc
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/temperature/fog.voc
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/temperature/high.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/temperature/hot.voc
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/temperature/low.voc
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/temperature/temperature.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.714939 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/unit/fahrenheit.voc
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/unit/unit.entity
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/unit/unit.voc
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/locale/sv-se/vocabulary/weather.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.714939 neon-skill-weather-2.0.1a1/neon_skill_weather.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-14 01:06:51.000000 neon-skill-weather-2.0.1a1/neon_skill_weather.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    67906 2024-05-14 01:06:51.000000 neon-skill-weather-2.0.1a1/neon_skill_weather.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 01:06:51.000000 neon-skill-weather-2.0.1a1/neon_skill_weather.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 01:06:51.000000 neon-skill-weather-2.0.1a1/neon_skill_weather.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-14 01:06:51.000000 neon-skill-weather-2.0.1a1/neon_skill_weather.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 01:06:51.000000 neon-skill-weather-2.0.1a1/neon_skill_weather.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 01:06:51.722939 neon-skill-weather-2.0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.714939 neon-skill-weather-2.0.1a1/skill/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/skill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/skill/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/skill/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16568 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/skill/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/skill/intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/skill/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/skill/weather.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.718939 neon-skill-weather-2.0.1a1/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/DailyColumn.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/DailyColumnScalable.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/DailyDelegateScalable.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/HourlyColumn.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/WeatherDate.qml
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/WeatherDelegateMarkII.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/WeatherDelegateScalable.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/WeatherImage.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/WeatherLabel.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/WeatherLocation.qml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.718939 neon-skill-weather-2.0.1a1/ui/animations/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4829 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/animations/clouds.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     5635 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/animations/fog.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     8559 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/animations/partial_clouds.json
--rwxr-xr-x   0 runner    (1001) docker     (127)    64205 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/animations/rain.json
--rwxr-xr-x   0 runner    (1001) docker     (127)    30103 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/animations/sleet.json
--rwxr-xr-x   0 runner    (1001) docker     (127)    46868 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/animations/snow.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     4248 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/animations/storm.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     4811 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/animations/sun.json
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/current_1_mark_ii.qml
--rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/current_1_scalable.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/current_2_mark_ii.qml
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/current_2_scalable.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/daily_mark_ii.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/daily_scalable.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/hourly_mark_ii.qml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:06:51.722939 neon-skill-weather-2.0.1a1/ui/images/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/images/clouds.svg
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/images/fog.svg
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/images/high_temperature.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/images/humidity.svg
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/images/low_temperature.svg
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/images/moon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/images/partial_clouds_day.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/images/partial_clouds_night.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/images/rain.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/images/snow.svg
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/images/storm.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/images/sun.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/images/sunrise.svg
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/images/sunset.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/images/wind.svg
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/qmldir
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/single_day_mark_ii.qml
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/ui/sunrise_sunset_mark_ii.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-14 01:06:48.000000 neon-skill-weather-2.0.1a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.563100 neon-skill-weather-2.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-15 19:16:38.563100 neon-skill-weather-2.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    48845 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.367096 neon-skill-weather-2.0.1a2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.351095 neon-skill-weather-2.0.1a2/locale/ca-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.371096 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/and.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.371096 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/condition/clear sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.375096 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/current/current-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.379096 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/daily-wind-light-loaction.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.379096 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.379096 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/error/location-not-found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/error/no-forecast.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.379096 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.383096 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.383096 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/weekly/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/dialog/weekly/weekly-temperature.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.383096 neon-skill-weather-2.0.1a2/locale/ca-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.383096 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.383096 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/condition/do.i.need.an.umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.383096 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.387096 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.387096 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.387096 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ca-es/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.351095 neon-skill-weather-2.0.1a2/locale/da-dk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.387096 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/and.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.387096 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/condition/clear sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.391096 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.395096 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.395096 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.395096 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/error/location-not-found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/error/no-forecast.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.395096 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.395096 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.399096 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/weekly/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/dialog/weekly/weekly-temperature.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.399096 neon-skill-weather-2.0.1a2/locale/da-dk/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.399096 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.399096 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/condition/do-i-need-an-umbrella-intent
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.399096 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.403096 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.403096 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.403096 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/da-dk/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.355095 neon-skill-weather-2.0.1a2/locale/de-de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.403096 neon-skill-weather-2.0.1a2/locale/de-de/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/and.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.403096 neon-skill-weather-2.0.1a2/locale/de-de/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/condition/clear sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.407096 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-humidity-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/current/current-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.411097 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.415097 neon-skill-weather-2.0.1a2/locale/de-de/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.415097 neon-skill-weather-2.0.1a2/locale/de-de/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/error/location-not-found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/error/no-forecast.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.415097 neon-skill-weather-2.0.1a2/locale/de-de/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.415097 neon-skill-weather-2.0.1a2/locale/de-de/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.415097 neon-skill-weather-2.0.1a2/locale/de-de/dialog/weekly/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/weekly/weekly-condition.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/dialog/weekly/weekly-temperature.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.415097 neon-skill-weather-2.0.1a2/locale/de-de/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.419097 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.419097 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/condition/do.i.need.an.umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.419097 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.423097 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.423097 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.423097 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/de-de/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.355095 neon-skill-weather-2.0.1a2/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.423097 neon-skill-weather-2.0.1a2/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/and.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.423097 neon-skill-weather-2.0.1a2/locale/en-us/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/condition/clear-sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/condition/clouds.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/condition/humidity.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.427097 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-humidity-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/current/currrent-clouds-alternative-local.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.431097 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.435097 neon-skill-weather-2.0.1a2/locale/en-us/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.435097 neon-skill-weather-2.0.1a2/locale/en-us/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/error/location-not-found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/error/no-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/error/seven-days-available.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.435097 neon-skill-weather-2.0.1a2/locale/en-us/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.435097 neon-skill-weather-2.0.1a2/locale/en-us/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.435097 neon-skill-weather-2.0.1a2/locale/en-us/dialog/weekly/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/weekly/weekly-condition.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/dialog/weekly/weekly-temperature.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.435097 neon-skill-weather-2.0.1a2/locale/en-us/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.439097 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.439097 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.439097 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/date-time/few.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/date-time/number-days.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/like.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/location.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/outside.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.443097 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.443097 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.443097 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/en-us/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.355095 neon-skill-weather-2.0.1a2/locale/es-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.443097 neon-skill-weather-2.0.1a2/locale/es-es/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.443097 neon-skill-weather-2.0.1a2/locale/es-es/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/condition/humidity.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/condition/snow.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.443097 neon-skill-weather-2.0.1a2/locale/es-es/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/current/current-weather-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.443097 neon-skill-weather-2.0.1a2/locale/es-es/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/daily/daily-weather-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.447097 neon-skill-weather-2.0.1a2/locale/es-es/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.447097 neon-skill-weather-2.0.1a2/locale/es-es/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/error/location-not-found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.447097 neon-skill-weather-2.0.1a2/locale/es-es/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.447097 neon-skill-weather-2.0.1a2/locale/es-es/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.447097 neon-skill-weather-2.0.1a2/locale/es-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.447097 neon-skill-weather-2.0.1a2/locale/es-es/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.447097 neon-skill-weather-2.0.1a2/locale/es-es/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.447097 neon-skill-weather-2.0.1a2/locale/es-es/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.447097 neon-skill-weather-2.0.1a2/locale/es-es/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/vocabulary/sunset.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/es-es/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.359095 neon-skill-weather-2.0.1a2/locale/eu-eu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.447097 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.451097 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/condition/clear-sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/condition/clouds.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/condition/humidity.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.455098 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-humidity-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/current/currrent-clouds-alternative-local.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.459098 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.459098 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.459098 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/error/location-not-found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/error/no-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/error/seven-days-available.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.463098 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.463098 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.463098 neon-skill-weather-2.0.1a2/locale/eu-eu/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.463098 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.463098 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.467098 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/date-time/few.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/date-time/number-days.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.467098 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.467098 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.467098 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.359095 neon-skill-weather-2.0.1a2/locale/fr-fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.467098 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.467098 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/condition/snow.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.471098 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/current/current-weather-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.471098 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/daily/daily-weather-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.471098 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.471098 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/error/location-not-found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.471098 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.471098 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.471098 neon-skill-weather-2.0.1a2/locale/fr-fr/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.471098 neon-skill-weather-2.0.1a2/locale/fr-fr/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.471098 neon-skill-weather-2.0.1a2/locale/fr-fr/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.475098 neon-skill-weather-2.0.1a2/locale/fr-fr/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.475098 neon-skill-weather-2.0.1a2/locale/fr-fr/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/vocabulary/sunset.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/fr-fr/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.359095 neon-skill-weather-2.0.1a2/locale/gl-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.475098 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/and.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.475098 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/condition/clear sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/condition/percentage-number.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.479098 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/current/current-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.479098 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.483098 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.483098 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/error/location-not-found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/error/no-forecast.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.483098 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/hourly/hourly-condition-expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.483098 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.483098 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/weekly/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/dialog/weekly/weekly-temperature.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.483098 neon-skill-weather-2.0.1a2/locale/gl-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.483098 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.487098 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/condition/do.i.need.an.umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.487098 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.487098 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.487098 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.491098 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/gl-es/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.363095 neon-skill-weather-2.0.1a2/locale/it-it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.491098 neon-skill-weather-2.0.1a2/locale/it-it/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.491098 neon-skill-weather-2.0.1a2/locale/it-it/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/condition/snow.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.491098 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/current/current-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.495098 neon-skill-weather-2.0.1a2/locale/it-it/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.495098 neon-skill-weather-2.0.1a2/locale/it-it/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.495098 neon-skill-weather-2.0.1a2/locale/it-it/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/error/location-not-found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.495098 neon-skill-weather-2.0.1a2/locale/it-it/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.499099 neon-skill-weather-2.0.1a2/locale/it-it/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.499099 neon-skill-weather-2.0.1a2/locale/it-it/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.499099 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.499099 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/condition/do.i.need.an.umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.499099 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.499099 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.503099 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.503099 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/it-it/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.363095 neon-skill-weather-2.0.1a2/locale/nl-nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.503099 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.503099 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/condition/snow.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.503099 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/current/current-weather-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.503099 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/daily/daily-weather-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.503099 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/direction/southwest.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.503099 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/error/location-not-found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.503099 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.507099 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.507099 neon-skill-weather-2.0.1a2/locale/nl-nl/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.507099 neon-skill-weather-2.0.1a2/locale/nl-nl/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.507099 neon-skill-weather-2.0.1a2/locale/nl-nl/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.507099 neon-skill-weather-2.0.1a2/locale/nl-nl/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.507099 neon-skill-weather-2.0.1a2/locale/nl-nl/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/vocabulary/sunset.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/nl-nl/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.367096 neon-skill-weather-2.0.1a2/locale/pt-br/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.507099 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/and.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.507099 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/condition/clear sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.511099 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/current/current-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.515099 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/daily/daily-temperature-high.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.515099 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.515099 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/error/location-not-found.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.515099 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.515099 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.515099 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/weekly/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/dialog/weekly/weekly-temperature.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.515099 neon-skill-weather-2.0.1a2/locale/pt-br/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.519099 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.519099 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/condition/do.i.need.an.umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.519099 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.523099 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.523099 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.523099 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/pt-br/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.367096 neon-skill-weather-2.0.1a2/locale/ru-ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.523099 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/and.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.523099 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/condition/clear-sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/condition/clouds.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/condition/humidity.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.527099 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-humidity-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-sunrise-future-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-sunrise-future-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-sunrise-past-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-sunrise-past-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-sunset-future-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-sunset-future-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-sunset-past-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-sunset-past-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-wind-strong-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/currrent-clouds-alternative-local.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.531099 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-humidity-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-precipitation-next-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-precipitation-next-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-precipitation-next-none-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-precipitation-next-none-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-sunrise-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-sunrise-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-sunset-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-sunset-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-weather-loation.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.535099 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.535099 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/error/forty-eight-hours-available.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/error/location-not-found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/error/no-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/error/seven-days-available.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.535099 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/hourly/hourly-precipitation-next-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/hourly/hourly-precipitation-next-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/hourly/hourly-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.535099 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.535099 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/weekly/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/weekly/weekly-condition.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/weekly/weekly-temperature.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.535099 neon-skill-weather-2.0.1a2/locale/ru-ru/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.539099 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.539099 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/condition/do-i-need-an-umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/condition/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.539099 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/date-time/few.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/date-time/number-days.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/like.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/location.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/outside.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.539099 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.543099 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.543099 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.367096 neon-skill-weather-2.0.1a2/locale/sv-se/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.543099 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/and.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.543099 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/condition/clear sky.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/condition/clear.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/condition/no precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/condition/precipitation expected.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/condition/rain.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/condition/snow.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/condition/thunderstorm.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.543099 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-humidity-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-temperature-high-low.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/current/current-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.547100 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/daily-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/daily-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/daily-temperature-high-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/daily-temperature-high-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/daily-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/daily-temperature-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/daily-temperature-low-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/daily-temperature-low-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/daily-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/daily-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/daily-wind-light-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/daily-wind-light-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/daily-wind-moderate-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/daily-wind-moderate-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/daily-wind-strong-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/daily-wind-strong-location.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.547100 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/direction/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/direction/east.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/direction/north.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/direction/northeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/direction/northwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/direction/south.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/direction/southeast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/direction/southwest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/direction/west.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.547100 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/error/cant-get-forecast.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/error/location-not-found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/error/no-forecast.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.547100 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/hourly/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/hourly/hourly-condition-alternative-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/hourly/hourly-condition-alternative-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/hourly/hourly-condition-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/hourly/hourly-condition-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/hourly/hourly-condition-not-expected-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/hourly/hourly-condition-not-expected-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/hourly/hourly-temperature-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/hourly/hourly-weather-local.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/hourly/hourly-weather-location.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/percentage-number.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.551100 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/unit/celsius.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/unit/fahrenheit.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/unit/meters per second.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/unit/miles per hour.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.551100 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/weekly/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/dialog/weekly/weekly-temperature.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.551100 neon-skill-weather-2.0.1a2/locale/sv-se/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/regex/location.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.551100 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.551100 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/condition/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/condition/clear.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/condition/clouds.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/condition/do.i.need.an.umbrella.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/condition/humidity.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/condition/precipitation.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/condition/rain.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/condition/snow.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/condition/thunderstorm.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/condition/windy.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.551100 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/date-time/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/date-time/couple.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/date-time/later.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/date-time/next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/date-time/now.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/date-time/relative-day.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/date-time/relative-time.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/date-time/today.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/date-time/week.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/date-time/weekend.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/forecast.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/location.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.555100 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/query/confirm-query-current.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/query/confirm-query-future.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/query/confirm-query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/query/how.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/query/query.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/query/when.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/sunrise.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/sunset.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.555100 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/temperature/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/temperature/cold.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/temperature/fog.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/temperature/high.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/temperature/hot.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/temperature/low.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/temperature/temperature.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.555100 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/unit/fahrenheit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/unit/unit.entity
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/unit/unit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/locale/sv-se/vocabulary/weather.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.555100 neon-skill-weather-2.0.1a2/neon_skill_weather.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-15 19:16:38.000000 neon-skill-weather-2.0.1a2/neon_skill_weather.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    67906 2024-05-15 19:16:38.000000 neon-skill-weather-2.0.1a2/neon_skill_weather.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:16:38.000000 neon-skill-weather-2.0.1a2/neon_skill_weather.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:16:38.000000 neon-skill-weather-2.0.1a2/neon_skill_weather.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 19:16:38.000000 neon-skill-weather-2.0.1a2/neon_skill_weather.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:16:38.000000 neon-skill-weather-2.0.1a2/neon_skill_weather.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:16:38.563100 neon-skill-weather-2.0.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.555100 neon-skill-weather-2.0.1a2/skill/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/skill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/skill/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/skill/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/skill/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/skill/intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/skill/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/skill/weather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.559100 neon-skill-weather-2.0.1a2/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/DailyColumn.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/DailyColumnScalable.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/DailyDelegateScalable.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/HourlyColumn.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/WeatherDate.qml
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/WeatherDelegateMarkII.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/WeatherDelegateScalable.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/WeatherImage.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/WeatherLabel.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/WeatherLocation.qml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.559100 neon-skill-weather-2.0.1a2/ui/animations/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4829 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/animations/clouds.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5635 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/animations/fog.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8559 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/animations/partial_clouds.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)    64205 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/animations/rain.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30103 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/animations/sleet.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46868 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/animations/snow.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4248 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/animations/storm.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4811 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/animations/sun.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/current_1_mark_ii.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/current_1_scalable.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/current_2_mark_ii.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/current_2_scalable.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/daily_mark_ii.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/daily_scalable.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/hourly_mark_ii.qml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:16:38.563100 neon-skill-weather-2.0.1a2/ui/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/images/clouds.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/images/fog.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/images/high_temperature.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/images/humidity.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/images/low_temperature.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/images/moon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/images/partial_clouds_day.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/images/partial_clouds_night.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/images/rain.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/images/snow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/images/storm.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/images/sun.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/images/sunrise.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/images/sunset.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/images/wind.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/qmldir
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/single_day_mark_ii.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/ui/sunrise_sunset_mark_ii.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-15 19:16:34.000000 neon-skill-weather-2.0.1a2/version.py
```

### Comparing `neon-skill-weather-2.0.1a1/LICENSE` & `neon-skill-weather-2.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/LICENSE.md` & `neon-skill-weather-2.0.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/PKG-INFO` & `neon-skill-weather-2.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-weather
-Version: 2.0.1a1
+Version: 2.0.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-weather
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-weather-2.0.1a1/README.md` & `neon-skill-weather-2.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/__init__.py` & `neon-skill-weather-2.0.1a2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
 from datetime import datetime
 from pathlib import Path
 from threading import Event
 from time import time
 from typing import List, Tuple, Optional
 
+from neon_utils.location_utils import get_timezone
 from requests import HTTPError
 from ovos_bus_client.message import Message
 from ovos_utils import classproperty
 from ovos_utils.log import LOG
 from ovos_utils.process_utils import RuntimeRequirements
 from neon_utils.skills.neon_skill import NeonSkill
 from neon_utils.signal_utils import wait_for_signal_clear
@@ -134,18 +135,20 @@
         """Handles a message bus command requesting current local weather information.
 
         Such a request will typically come from a domain external to this skill that
         requires weather information but should not go through the intent system
         to get it.
         """
         system_unit = self.config_core.get("system_unit")
+        timezone = get_user_prefs(message)["location"]["timezone"]
         try:
             weather = self.weather_api.get_weather_for_coordinates(
                 system_unit, self._get_weather_config(message).latitude,
-                self._get_weather_config(message).longitude, self.lang
+                self._get_weather_config(message).longitude, self.lang,
+                timezone
             )
         except Exception:
             self.log.exception("Unexpected error getting weather.")
             self.bus.emit(Message("skill.weather.local-forecast-failure."))
         else:
             self._emit_local_weather_response(weather)
 
@@ -1130,16 +1133,17 @@
             An object representing the data returned by the API
         """
         weather = None
         if intent_data is not None:
             try:
                 unit = get_user_prefs()['units']['measure']
                 latitude, longitude = self._determine_weather_location(intent_data)
+                timezone, _ = get_timezone(latitude, longitude)
                 weather = self.weather_api.get_weather_for_coordinates(
-                    unit, latitude, longitude, self.lang
+                    unit, latitude, longitude, self.lang, timezone
                 )
             except HTTPError as api_error:
                 self.log.exception("Weather API failure")
                 self._handle_api_error(api_error)
             except LocationNotFoundError:
                 self.log.exception("City not found.")
                 self.speak_dialog(
```

### Comparing `neon-skill-weather-2.0.1a1/locale/ca-es/dialog/daily/daily-weather-local.dialog` & `neon-skill-weather-2.0.1a2/locale/ca-es/dialog/daily/daily-weather-local.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/locale/da-dk/dialog/current/current-weather-location.dialog` & `neon-skill-weather-2.0.1a2/locale/da-dk/dialog/current/current-weather-location.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-weather-local.dialog` & `neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-weather-local.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/locale/da-dk/dialog/daily/daily-weather-location.dialog` & `neon-skill-weather-2.0.1a2/locale/da-dk/dialog/daily/daily-weather-location.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/locale/da-dk/dialog/hourly/hourly-weather-location.dialog` & `neon-skill-weather-2.0.1a2/locale/da-dk/dialog/hourly/hourly-weather-location.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/locale/es-es/dialog/current/current-weather-local.dialog` & `neon-skill-weather-2.0.1a2/locale/es-es/dialog/current/current-weather-local.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/locale/es-es/dialog/current/current-weather-location.dialog` & `neon-skill-weather-2.0.1a2/locale/es-es/dialog/current/current-weather-location.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/locale/eu-eu/vocabulary/location.voc` & `neon-skill-weather-2.0.1a2/locale/eu-eu/vocabulary/location.voc`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/current/current-weather-local.dialog` & `neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/current/current-weather-local.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/locale/fr-fr/dialog/current/current-weather-location.dialog` & `neon-skill-weather-2.0.1a2/locale/fr-fr/dialog/current/current-weather-location.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/locale/nl-nl/dialog/current/current-weather-local.dialog` & `neon-skill-weather-2.0.1a2/locale/nl-nl/dialog/current/current-weather-local.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/locale/ru-ru/dialog/current/current-weather-location.dialog` & `neon-skill-weather-2.0.1a2/locale/ru-ru/dialog/current/current-weather-location.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/locale/ru-ru/vocabulary/date-time/number-days.voc` & `neon-skill-weather-2.0.1a2/locale/ru-ru/vocabulary/date-time/number-days.voc`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/locale/sv-se/dialog/daily/daily-weather-local.dialog` & `neon-skill-weather-2.0.1a2/locale/sv-se/dialog/daily/daily-weather-local.dialog`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/neon_skill_weather.egg-info/PKG-INFO` & `neon-skill-weather-2.0.1a2/neon_skill_weather.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-weather
-Version: 2.0.1a1
+Version: 2.0.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-weather
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-weather-2.0.1a1/neon_skill_weather.egg-info/SOURCES.txt` & `neon-skill-weather-2.0.1a2/neon_skill_weather.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/setup.py` & `neon-skill-weather-2.0.1a2/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/skill/__init__.py` & `neon-skill-weather-2.0.1a2/skill/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/skill/api.py` & `neon-skill-weather-2.0.1a2/skill/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,27 +125,29 @@
                         "lang_code": lang}
         forecast = request_backend("proxy/weather", request_data)
         formatted = {"main": forecast["current"], "weather": forecast["current"]["weather"]}
         return formatted
 
     def get_weather_for_coordinates(
         self, measurement_system: str, latitude: float,
-        longitude: float, lang: str
+        longitude: float, lang: str, timezone: str
     ) -> WeatherReport:
         """Issue an API call and map the return value into a weather report
 
         Args:
             measurement_system: Metric or Imperial measurement units
             latitude: the geologic latitude of the weather location
             longitude: the geologic longitude of the weather location
             lang: language requested
+            timezone: timezone to use for returned WeatherReport
         """
         lang = lang or self.language
         if not self.lang == lang:
             self.lang = lang
             # self.set_language_parameter(lang)
         request_data = {"api": "onecall", "lat": latitude, "lon": longitude, "unit": measurement_system,
                         "lang_code": lang}
         forecast = request_backend("proxy/weather", request_data)
+        forecast["timezone"] = timezone
         local_weather = WeatherReport(forecast)
 
         return local_weather
```

### Comparing `neon-skill-weather-2.0.1a1/skill/config.py` & `neon-skill-weather-2.0.1a2/skill/config.py`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/skill/dialog.py` & `neon-skill-weather-2.0.1a2/skill/dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,29 +29,31 @@
         example, temperature can be qualified by "high" or "low".
     * Locale: indicates if the dialog is for local weather or weather in a remote
         location.
 
 The skill class will use the "name" and "data" attributes to pass to the TTS process.
 """
 from typing import List, Tuple
+from datetime import datetime
+from lingua_franca.format import join_list, nice_number, nice_time
+from ovos_utils import LOG
 
-from mycroft.util.format import join_list, nice_number, nice_time
-from mycroft.util.time import now_local
 from .config import WeatherConfig
 from .intent import WeatherIntent
 from .util import get_speakable_day_of_week, get_time_period
 from .weather import (
     CURRENT,
     CurrentWeather,
     DAILY,
     DailyWeather,
     HOURLY,
     HourlyWeather,
 )
 
+
 # TODO: MISSING DIALOGS
 #   - current.clear.alternative.local
 #   - current.clouds.alternative.local
 #   - daily.snow.alternative.local
 #   - all hourly.<condition>.alternative.local/location
 #   - all hourly.<condition>.not.expected.local/location
 class WeatherDialog:
@@ -148,30 +150,28 @@
                 self.weather.condition.category.lower()
             )
         self._add_location()
 
     def build_sunrise_dialog(self):
         """Build the components necessary to speak the sunrise time."""
         if self.intent_data.location is None:
-            now = now_local()
+            LOG.warning(f"No location to determine timezone!")
+            now = datetime.now(tz=self.weather.date_time.tzinfo)
         else:
-            now = now_local(tz=self.intent_data.geolocation["timezone"])
+            now = datetime.now(tz=self.intent_data.geolocation["timezone"])
         if now < self.weather.sunrise:
             self.name += "-sunrise-future"
         else:
             self.name += "-sunrise-past"
         self.data = dict(time=nice_time(self.weather.sunrise))
         self._add_location()
 
     def build_sunset_dialog(self):
         """Build the components necessary to speak the sunset time."""
-        if self.intent_data.location is None:
-            now = now_local()
-        else:
-            now = now_local(tz=self.intent_data.geolocation["timezone"])
+        now = datetime.now(tz=self.weather.date_time.tzinfo)
         if now < self.weather.sunset:
             self.name += "-sunset-future"
         else:
             self.name += "-sunset-past"
         self.data = dict(time=nice_time(self.weather.sunset))
         self._add_location()
```

### Comparing `neon-skill-weather-2.0.1a1/skill/intent.py` & `neon-skill-weather-2.0.1a2/skill/intent.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Parse the intent into data used by the weather skill."""
-from datetime import timedelta
 
 import pytz
-from mycroft.util.time import now_local
+from ovos_config.locale import get_default_tz
+from datetime import datetime, timedelta
 from neon_utils.location_utils import get_coordinates, get_location, get_timezone
 
 from .util import (
     get_utterance_datetime,
     # get_geolocation,
     get_tz_info,
     LocationNotFoundError,
@@ -110,13 +110,13 @@
         """Determine the current date and time for the request.
 
         If a location is specified in the request, use the timezone for that
         location, otherwise, use the timezone configured on the device.
         """
         if self._location_datetime is None:
             if self.location is None:
-                self._location_datetime = now_local()
+                self._location_datetime = datetime.now(get_default_tz())
             else:
                 tz_info = get_tz_info(self.geolocation["timezone"])
-                self._location_datetime = now_local(tz_info)
+                self._location_datetime = datetime.now(tz_info)
 
         return self._location_datetime
```

### Comparing `neon-skill-weather-2.0.1a1/skill/util.py` & `neon-skill-weather-2.0.1a2/skill/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Utility functions for the weather skill."""
-from datetime import datetime, timedelta, tzinfo
-from time import time
 
 import pytz
 
-from mycroft.api import GeolocationApi
-from mycroft.util.format import nice_date
-from mycroft.util.parse import extract_datetime
-from mycroft.util.time import now_local
+from datetime import datetime, timedelta, tzinfo
+from time import time
+from ovos_backend_client.api import GeolocationApi
+from lingua_franca.format import nice_date
+from lingua_franca.parse import extract_datetime
+from ovos_config.locale import get_default_tz
+
 
 
 class LocationNotFoundError(ValueError):
     """Raise when the API cannot find the requested location."""
 
     pass
 
@@ -137,15 +138,16 @@
 
     Args:
         date_to_speak: The date/time for the forecast being reported.
 
     Returns:
         The day of the week in the device's configured language
     """
-    now = now_local()
+    tz = date_to_speak.tzinfo or get_default_tz()
+    now = datetime.now(tz)
     tomorrow = now.date() + timedelta(days=1)
 
     # A little hack to prevent nice_date() from returning "tomorrow"
     if date_to_speak.date() == tomorrow:
         now_arg = now - timedelta(days=1)
     else:
         now_arg = now
```

### Comparing `neon-skill-weather-2.0.1a1/skill/weather.py` & `neon-skill-weather-2.0.1a2/skill/weather.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Representations and conversions of the data returned by the weather API."""
-from datetime import timedelta
+
+import pytz
+
+from datetime import datetime, timedelta
 from pathlib import Path
 from typing import List
-from neon_utils.logger import LOG
+from ovos_utils.log import LOG
 
 from .config import MILES_PER_HOUR
 from .util import convert_to_local_datetime
 
 # Forecast timeframes
 CURRENT = "current"
 DAILY = "daily"
@@ -178,16 +181,17 @@
 
 
 class CurrentWeather(Weather):
     """Data representation of the current weather returned by the API"""
 
     def __init__(self, weather: dict, timezone: str):
         super().__init__(weather, timezone)
-        self.sunrise = convert_to_local_datetime(weather["sunrise"], timezone)
-        self.sunset = convert_to_local_datetime(weather["sunset"], timezone)
+        timezone = pytz.timezone(timezone)
+        self.sunrise = datetime.fromtimestamp(weather["sunrise"], tz=timezone)
+        self.sunset = datetime.fromtimestamp(weather["sunset"], tz=timezone)
         self.temperature = round(weather["temp"])
         self.visibility = weather["visibility"]
         self.low_temperature = None
         self.high_temperature = None
 
 
 class DailyFeelsLike:
@@ -245,14 +249,15 @@
     """Full representation of the data returned by the Open Weather Maps One Call API"""
 
     def __init__(self, report: dict):
         if "error" in report:
             LOG.error(report)
             raise Exception(report.get('content'))
         timezone = report["timezone"]
+        LOG.info(f"Weather report for timezone: {timezone}")
         self.current = CurrentWeather(report["current"], timezone)
         self.hourly = [HourlyWeather(hour, timezone) for hour in report.get("hourly", list())]
         self.daily = [DailyWeather(day, timezone) for day in report.get("daily", list())]
         today = self.daily[0]
         self.current.high_temperature = today.temperature.high
         self.current.low_temperature = today.temperature.low
         if "alerts" in report:
```

### Comparing `neon-skill-weather-2.0.1a1/skill.json` & `neon-skill-weather-2.0.1a2/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/DailyColumn.qml` & `neon-skill-weather-2.0.1a2/ui/DailyColumn.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/DailyColumnScalable.qml` & `neon-skill-weather-2.0.1a2/ui/DailyColumnScalable.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/DailyDelegateScalable.qml` & `neon-skill-weather-2.0.1a2/ui/DailyDelegateScalable.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/HourlyColumn.qml` & `neon-skill-weather-2.0.1a2/ui/HourlyColumn.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/WeatherDate.qml` & `neon-skill-weather-2.0.1a2/ui/WeatherDate.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/WeatherDelegateMarkII.qml` & `neon-skill-weather-2.0.1a2/ui/WeatherDelegateMarkII.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/WeatherDelegateScalable.qml` & `neon-skill-weather-2.0.1a2/ui/WeatherDelegateScalable.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/WeatherImage.qml` & `neon-skill-weather-2.0.1a2/ui/WeatherImage.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/WeatherLabel.qml` & `neon-skill-weather-2.0.1a2/ui/WeatherLabel.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/WeatherLocation.qml` & `neon-skill-weather-2.0.1a2/ui/WeatherLocation.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/animations/clouds.json` & `neon-skill-weather-2.0.1a2/ui/animations/clouds.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/animations/fog.json` & `neon-skill-weather-2.0.1a2/ui/animations/fog.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/animations/partial_clouds.json` & `neon-skill-weather-2.0.1a2/ui/animations/partial_clouds.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/animations/rain.json` & `neon-skill-weather-2.0.1a2/ui/animations/rain.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/animations/sleet.json` & `neon-skill-weather-2.0.1a2/ui/animations/sleet.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/animations/snow.json` & `neon-skill-weather-2.0.1a2/ui/animations/snow.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/animations/storm.json` & `neon-skill-weather-2.0.1a2/ui/animations/storm.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/animations/sun.json` & `neon-skill-weather-2.0.1a2/ui/animations/sun.json`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/current_1_mark_ii.qml` & `neon-skill-weather-2.0.1a2/ui/current_1_mark_ii.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/current_1_scalable.qml` & `neon-skill-weather-2.0.1a2/ui/current_1_scalable.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/current_2_mark_ii.qml` & `neon-skill-weather-2.0.1a2/ui/current_2_mark_ii.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/current_2_scalable.qml` & `neon-skill-weather-2.0.1a2/ui/current_2_scalable.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/daily_mark_ii.qml` & `neon-skill-weather-2.0.1a2/ui/daily_mark_ii.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/daily_scalable.qml` & `neon-skill-weather-2.0.1a2/ui/daily_scalable.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/hourly_mark_ii.qml` & `neon-skill-weather-2.0.1a2/ui/hourly_mark_ii.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/images/clouds.svg` & `neon-skill-weather-2.0.1a2/ui/images/clouds.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/images/fog.svg` & `neon-skill-weather-2.0.1a2/ui/images/fog.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/images/high_temperature.svg` & `neon-skill-weather-2.0.1a2/ui/images/high_temperature.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/images/humidity.svg` & `neon-skill-weather-2.0.1a2/ui/images/humidity.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/images/low_temperature.svg` & `neon-skill-weather-2.0.1a2/ui/images/low_temperature.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/images/partial_clouds_day.svg` & `neon-skill-weather-2.0.1a2/ui/images/partial_clouds_day.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/images/partial_clouds_night.svg` & `neon-skill-weather-2.0.1a2/ui/images/partial_clouds_night.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/images/rain.svg` & `neon-skill-weather-2.0.1a2/ui/images/rain.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/images/snow.svg` & `neon-skill-weather-2.0.1a2/ui/images/snow.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/images/storm.svg` & `neon-skill-weather-2.0.1a2/ui/images/storm.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/images/sun.svg` & `neon-skill-weather-2.0.1a2/ui/images/sun.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/images/sunrise.svg` & `neon-skill-weather-2.0.1a2/ui/images/sunrise.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/images/sunset.svg` & `neon-skill-weather-2.0.1a2/ui/images/sunset.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/images/wind.svg` & `neon-skill-weather-2.0.1a2/ui/images/wind.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/single_day_mark_ii.qml` & `neon-skill-weather-2.0.1a2/ui/single_day_mark_ii.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/ui/sunrise_sunset_mark_ii.qml` & `neon-skill-weather-2.0.1a2/ui/sunrise_sunset_mark_ii.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-weather-2.0.1a1/version.py` & `neon-skill-weather-2.0.1a2/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.0.1a1"
+__version__ = "2.0.1a2"
```

