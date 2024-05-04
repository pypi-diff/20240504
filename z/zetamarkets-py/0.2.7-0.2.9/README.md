# Comparing `tmp/zetamarkets_py-0.2.7.tar.gz` & `tmp/zetamarkets_py-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zetamarkets_py-0.2.7.tar", max compression
+gzip compressed data, was "zetamarkets_py-0.2.9.tar", max compression
```

## Comparing `zetamarkets_py-0.2.7.tar` & `zetamarkets_py-0.2.9.tar`

### file list

```diff
@@ -1,495 +1,485 @@
--rw-r--r--   0        0        0    11357 2023-08-14 01:58:30.329630 zetamarkets_py-0.2.7/LICENSE
--rw-r--r--   0        0        0     1782 2023-10-24 13:28:51.142402 zetamarkets_py-0.2.7/README.md
--rw-r--r--   0        0        0     1520 2023-11-18 02:36:37.791193 zetamarkets_py-0.2.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-13 00:55:50.042915 zetamarkets_py-0.2.7/zetamarkets_py/__init__.py
--rw-r--r--   0        0        0    50108 2023-11-18 02:34:44.789824 zetamarkets_py-0.2.7/zetamarkets_py/client.py
--rw-r--r--   0        0        0    14870 2023-10-24 06:57:36.616058 zetamarkets_py-0.2.7/zetamarkets_py/constants.py
--rw-r--r--   0        0        0     7352 2023-11-18 02:34:07.126035 zetamarkets_py-0.2.7/zetamarkets_py/events.py
--rw-r--r--   0        0        0     6043 2023-10-24 14:30:30.242399 zetamarkets_py-0.2.7/zetamarkets_py/exchange.py
--rw-r--r--   0        0        0   212543 2023-10-24 06:57:36.617444 zetamarkets_py-0.2.7/zetamarkets_py/idl/zeta.json
--rw-r--r--   0        0        0    11913 2023-10-24 14:30:30.283034 zetamarkets_py-0.2.7/zetamarkets_py/market.py
--rw-r--r--   0        0        0     6927 2023-10-24 12:30:20.973776 zetamarkets_py-0.2.7/zetamarkets_py/orderbook.py
--rw-r--r--   0        0        0     3177 2023-10-22 02:53:08.878101 zetamarkets_py-0.2.7/zetamarkets_py/pda.py
--rw-r--r--   0        0        0     6484 2023-11-14 13:45:38.014070 zetamarkets_py-0.2.7/zetamarkets_py/risk.py
--rw-r--r--   0        0        0        0 2023-09-24 12:36:37.774834 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/__init__.py
--rw-r--r--   0        0        0      168 2023-09-24 12:41:35.940107 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      220 2023-09-08 10:53:15.637267 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/__pycache__/constants.cpython-39.pyc
--rw-r--r--   0        0        0      290 2023-09-14 06:08:29.746879 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/__pycache__/program_id.cpython-39.pyc
--rw-r--r--   0        0        0      144 2023-09-24 12:41:27.831694 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/__init__.py
--rw-r--r--   0        0        0      361 2023-09-24 12:41:35.940389 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4211 2023-09-07 08:41:22.879317 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/__pycache__/market.cpython-39.pyc
--rw-r--r--   0        0        0     4269 2023-09-24 12:41:35.944154 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/__pycache__/market_state.cpython-39.pyc
--rw-r--r--   0        0        0     2949 2023-09-14 06:08:29.750538 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/__pycache__/open_orders.cpython-39.pyc
--rw-r--r--   0        0        0     2362 2023-09-14 06:08:29.749038 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/__pycache__/orderbook.cpython-39.pyc
--rw-r--r--   0        0        0     2400 2023-09-14 06:08:29.751949 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/__pycache__/queue.cpython-39.pyc
--rw-r--r--   0        0        0     5994 2023-09-24 12:40:15.782815 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/market_state.py
--rw-r--r--   0        0        0     3605 2023-09-12 11:00:06.010934 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/open_orders.py
--rw-r--r--   0        0        0     2509 2023-09-12 11:00:06.011239 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/orderbook.py
--rw-r--r--   0        0        0     2284 2023-09-12 11:00:06.011458 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/queue.py
--rw-r--r--   0        0        0      114 2023-09-12 11:00:06.011860 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/program_id.py
--rw-r--r--   0        0        0      119 2023-09-12 11:00:06.012149 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/types/__init__.py
--rw-r--r--   0        0        0      334 2023-09-14 06:08:29.740649 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/types/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2465 2023-09-14 06:08:29.741420 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/types/__pycache__/account_flags.cpython-39.pyc
--rw-r--r--   0        0        0     2872 2023-09-16 07:26:20.093737 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/types/__pycache__/queue.cpython-39.pyc
--rw-r--r--   0        0        0     5223 2023-09-24 11:48:22.348153 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/types/__pycache__/slab.cpython-39.pyc
--rw-r--r--   0        0        0     3517 2023-09-12 11:00:06.012683 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/types/account_flags.py
--rw-r--r--   0        0        0     2872 2023-09-14 08:14:56.146607 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/types/queue.py
--rw-r--r--   0        0        0     5316 2023-09-24 09:10:25.609095 zetamarkets_py-0.2.7/zetamarkets_py/serum_client/types/slab.py
--rw-r--r--   0        0        0     1474 2023-09-14 06:08:29.753679 zetamarkets_py-0.2.7/zetamarkets_py/solana_client/accounts/__pycache__/clock.cpython-39.pyc
--rw-r--r--   0        0        0     1325 2023-09-12 11:00:06.013459 zetamarkets_py-0.2.7/zetamarkets_py/solana_client/accounts/clock.py
--rw-r--r--   0        0        0     4490 2023-11-14 13:45:38.014374 zetamarkets_py-0.2.7/zetamarkets_py/types.py
--rw-r--r--   0        0        0     4086 2023-10-24 12:19:55.145643 zetamarkets_py-0.2.7/zetamarkets_py/utils.py
--rw-r--r--   0        0        0      242 2023-08-13 11:25:54.547491 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/README.md
--rw-r--r--   0        0        0        0 2023-09-24 12:29:58.953532 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/__init__.py
--rw-r--r--   0        0        0      178 2023-08-14 03:44:39.758195 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      167 2023-09-24 12:32:46.713703 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      358 2023-08-14 03:44:39.901255 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/__pycache__/program_id.cpython-311.pyc
--rw-r--r--   0        0        0      289 2023-08-16 14:09:56.107760 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/__pycache__/program_id.cpython-39.pyc
--rw-r--r--   0        0        0      186 2023-09-24 12:24:42.495690 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__init__.py
--rw-r--r--   0        0        0     3685 2023-08-21 18:06:22.713829 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      434 2023-09-24 12:25:12.101200 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    11893 2023-08-22 22:09:31.466239 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/cross_margin_account.cpython-311.pyc
--rw-r--r--   0        0        0     6213 2023-09-05 04:34:42.078727 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/cross_margin_account.cpython-39.pyc
--rw-r--r--   0        0        0     6381 2023-08-22 22:10:16.308666 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/cross_margin_account_manager.cpython-311.pyc
--rw-r--r--   0        0        0     3854 2023-09-05 04:34:47.091489 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/cross_margin_account_manager.cpython-39.pyc
--rw-r--r--   0        0        0     4906 2023-08-22 22:09:46.139814 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/cross_open_orders_map.cpython-311.pyc
--rw-r--r--   0        0        0     2998 2023-09-05 04:34:47.092791 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/cross_open_orders_map.cpython-39.pyc
--rw-r--r--   0        0        0    13204 2023-08-21 18:06:22.777847 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/greeks.cpython-311.pyc
--rw-r--r--   0        0        0     6404 2023-09-05 04:34:47.094576 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/greeks.cpython-39.pyc
--rw-r--r--   0        0        0     4737 2023-08-21 18:06:22.779493 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/insurance_deposit_account.cpython-311.pyc
--rw-r--r--   0        0        0     2924 2023-09-05 04:34:47.096158 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/insurance_deposit_account.cpython-39.pyc
--rw-r--r--   0        0        0    11691 2023-08-21 18:06:22.780756 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/margin_account.cpython-311.pyc
--rw-r--r--   0        0        0     5696 2023-09-05 04:34:47.097615 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/margin_account.cpython-39.pyc
--rw-r--r--   0        0        0     4909 2023-08-21 18:06:22.781959 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/market_indexes.cpython-311.pyc
--rw-r--r--   0        0        0     2959 2023-09-05 04:34:47.099022 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/market_indexes.cpython-39.pyc
--rw-r--r--   0        0        0     5041 2023-08-21 18:06:22.782902 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/market_node.cpython-311.pyc
--rw-r--r--   0        0        0     3017 2023-09-05 04:34:47.100154 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/market_node.cpython-39.pyc
--rw-r--r--   0        0        0     4666 2023-08-21 18:06:22.783836 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/open_orders_map.cpython-311.pyc
--rw-r--r--   0        0        0     2852 2023-09-05 04:34:47.101239 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/open_orders_map.cpython-39.pyc
--rw-r--r--   0        0        0     6174 2023-08-21 18:06:22.784860 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/perp_sync_queue.cpython-311.pyc
--rw-r--r--   0        0        0     3671 2023-09-05 04:34:47.102331 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/perp_sync_queue.cpython-39.pyc
--rw-r--r--   0        0        0    27485 2023-08-21 18:06:22.786941 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/pricing.cpython-311.pyc
--rw-r--r--   0        0        0    12015 2023-09-14 06:08:29.758060 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/pricing.cpython-39.pyc
--rw-r--r--   0        0        0     5608 2023-08-21 18:06:22.788620 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/referral_account.cpython-311.pyc
--rw-r--r--   0        0        0     3331 2023-09-05 04:34:47.106419 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/referral_account.cpython-39.pyc
--rw-r--r--   0        0        0     5406 2023-08-21 18:06:22.789588 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/referrer_account.cpython-311.pyc
--rw-r--r--   0        0        0     3259 2023-09-05 04:34:47.107566 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/referrer_account.cpython-39.pyc
--rw-r--r--   0        0        0     5063 2023-08-21 18:06:22.790529 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/referrer_alias.cpython-311.pyc
--rw-r--r--   0        0        0     3047 2023-09-05 04:34:47.108865 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/referrer_alias.cpython-39.pyc
--rw-r--r--   0        0        0     4777 2023-08-21 18:06:22.791415 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/settlement_account.cpython-311.pyc
--rw-r--r--   0        0        0     2905 2023-09-05 04:34:47.109971 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/settlement_account.cpython-39.pyc
--rw-r--r--   0        0        0     4749 2023-08-21 18:06:22.792267 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/socialized_loss_account.cpython-311.pyc
--rw-r--r--   0        0        0     2921 2023-09-05 04:34:47.111085 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/socialized_loss_account.cpython-39.pyc
--rw-r--r--   0        0        0     8550 2023-08-21 18:06:22.793322 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/spread_account.cpython-311.pyc
--rw-r--r--   0        0        0     4688 2023-09-05 04:34:47.112454 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/spread_account.cpython-39.pyc
--rw-r--r--   0        0        0    14841 2023-08-21 18:06:22.794731 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/state.cpython-311.pyc
--rw-r--r--   0        0        0     7157 2023-09-14 06:08:29.760633 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/state.cpython-39.pyc
--rw-r--r--   0        0        0     4629 2023-08-21 18:06:22.796189 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/underlying.cpython-311.pyc
--rw-r--r--   0        0        0     2822 2023-09-05 04:34:47.116137 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/underlying.cpython-39.pyc
--rw-r--r--   0        0        0     4919 2023-08-21 18:06:22.797606 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_deposit_account.cpython-311.pyc
--rw-r--r--   0        0        0     3026 2023-09-05 04:34:47.117112 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_deposit_account.cpython-39.pyc
--rw-r--r--   0        0        0     4935 2023-08-21 18:06:22.798485 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_insurance_account.cpython-311.pyc
--rw-r--r--   0        0        0     3042 2023-09-05 04:34:47.118173 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_insurance_account.cpython-39.pyc
--rw-r--r--   0        0        0     4952 2023-08-21 18:06:22.799441 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_trading_fees_account.cpython-311.pyc
--rw-r--r--   0        0        0     3059 2023-09-05 04:34:47.119209 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_trading_fees_account.cpython-39.pyc
--rw-r--r--   0        0        0    16492 2023-08-21 18:06:22.800886 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/zeta_group.cpython-311.pyc
--rw-r--r--   0        0        0     7405 2023-09-05 04:34:47.120985 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/zeta_group.cpython-39.pyc
--rw-r--r--   0        0        0     8516 2023-08-22 22:06:52.629137 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/cross_margin_account.py
--rw-r--r--   0        0        0    17452 2023-09-12 11:00:06.014511 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/pricing.py
--rw-r--r--   0        0        0    14179 2023-09-12 11:00:06.014788 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/state.py
--rw-r--r--   0        0        0      887 2023-09-24 12:24:44.931139 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/__init__.py
--rw-r--r--   0        0        0     1754 2023-08-29 19:26:18.521414 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1169 2023-09-24 12:25:12.107723 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    30973 2023-08-29 18:24:52.982819 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/__pycache__/anchor.cpython-311.pyc
--rw-r--r--   0        0        0    19297 2023-09-05 04:34:51.340870 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/__pycache__/anchor.cpython-39.pyc
--rw-r--r--   0        0        0    88246 2023-08-29 18:24:52.989435 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/__pycache__/custom.cpython-311.pyc
--rw-r--r--   0        0        0    55917 2023-09-05 04:34:51.346377 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/__pycache__/custom.cpython-39.pyc
--rw-r--r--   0        0        0    16145 2023-08-21 13:18:23.450876 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/anchor.py
--rw-r--r--   0        0        0    47202 2023-08-21 13:18:23.447398 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/custom.py
--rw-r--r--   0        0        0     2819 2023-09-24 12:24:47.366668 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__init__.py
--rw-r--r--   0        0        0    16417 2023-08-22 00:24:54.436216 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2723 2023-09-24 12:25:12.111529 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1560 2023-08-22 00:24:54.436812 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/add_market_indexes.cpython-311.pyc
--rw-r--r--   0        0        0     1114 2023-09-05 04:34:51.350580 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/add_market_indexes.cpython-39.pyc
--rw-r--r--   0        0        0     2236 2023-08-22 00:24:54.437323 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/add_perp_market_index.cpython-311.pyc
--rw-r--r--   0        0        0     1480 2023-09-05 04:34:51.351219 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/add_perp_market_index.cpython-39.pyc
--rw-r--r--   0        0        0     2211 2023-08-22 00:24:54.437941 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/apply_perp_funding.cpython-311.pyc
--rw-r--r--   0        0        0     1460 2023-09-05 04:34:51.351889 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/apply_perp_funding.cpython-39.pyc
--rw-r--r--   0        0        0     1899 2023-08-22 00:24:54.438531 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/burn_vault_tokens.cpython-311.pyc
--rw-r--r--   0        0        0     1272 2023-09-05 04:34:51.352393 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/burn_vault_tokens.cpython-39.pyc
--rw-r--r--   0        0        0     3631 2023-08-22 00:24:54.439068 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_all_market_orders.cpython-311.pyc
--rw-r--r--   0        0        0     2129 2023-09-05 04:34:51.353010 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_all_market_orders.cpython-39.pyc
--rw-r--r--   0        0        0     3888 2023-08-22 00:24:54.439608 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order.cpython-311.pyc
--rw-r--r--   0        0        0     2233 2023-09-05 04:34:51.353844 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order.cpython-39.pyc
--rw-r--r--   0        0        0     3787 2023-08-22 00:24:54.440148 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_by_client_order_id.cpython-311.pyc
--rw-r--r--   0        0        0     2228 2023-09-05 04:34:51.354577 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_by_client_order_id.cpython-39.pyc
--rw-r--r--   0        0        0     3819 2023-08-22 00:24:54.440786 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_by_client_order_id_no_error.cpython-311.pyc
--rw-r--r--   0        0        0     2260 2023-09-05 04:34:51.355440 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_by_client_order_id_no_error.cpython-39.pyc
--rw-r--r--   0        0        0     3802 2023-08-22 00:24:54.441360 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_halted.cpython-311.pyc
--rw-r--r--   0        0        0     2210 2023-09-05 04:34:51.356261 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_halted.cpython-39.pyc
--rw-r--r--   0        0        0     3920 2023-08-22 00:24:54.441941 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_no_error.cpython-311.pyc
--rw-r--r--   0        0        0     2265 2023-09-05 04:34:51.356941 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_no_error.cpython-39.pyc
--rw-r--r--   0        0        0     2074 2023-08-22 00:24:54.442349 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/claim_referrals_rewards.cpython-311.pyc
--rw-r--r--   0        0        0     1377 2023-09-05 04:34:51.357533 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/claim_referrals_rewards.cpython-39.pyc
--rw-r--r--   0        0        0     2431 2023-08-22 00:24:54.442726 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/clean_zeta_market_halted.cpython-311.pyc
--rw-r--r--   0        0        0     1560 2023-09-05 04:34:51.358036 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/clean_zeta_market_halted.cpython-39.pyc
--rw-r--r--   0        0        0     1546 2023-08-22 00:24:54.443264 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/clean_zeta_markets.cpython-311.pyc
--rw-r--r--   0        0        0     1105 2023-09-05 04:34:51.358697 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/clean_zeta_markets.cpython-39.pyc
--rw-r--r--   0        0        0     2281 2023-08-22 00:24:54.443819 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_cross_margin_account.cpython-311.pyc
--rw-r--r--   0        0        0     1521 2023-09-05 04:34:51.359308 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_cross_margin_account.cpython-39.pyc
--rw-r--r--   0        0        0     1628 2023-08-22 00:24:54.444234 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_cross_margin_account_manager.cpython-311.pyc
--rw-r--r--   0        0        0     1181 2023-09-05 04:34:51.359797 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_cross_margin_account_manager.cpython-39.pyc
--rw-r--r--   0        0        0     1673 2023-08-22 00:24:54.444537 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_margin_account.cpython-311.pyc
--rw-r--r--   0        0        0     1164 2023-09-05 04:34:51.360201 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_margin_account.cpython-39.pyc
--rw-r--r--   0        0        0     2849 2023-08-22 00:24:54.444993 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders.cpython-311.pyc
--rw-r--r--   0        0        0     1721 2023-09-05 04:34:51.360793 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders.cpython-39.pyc
--rw-r--r--   0        0        0     2750 2023-08-22 00:24:54.445492 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders_v2.cpython-311.pyc
--rw-r--r--   0        0        0     1686 2023-09-05 04:34:51.361413 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders_v2.cpython-39.pyc
--rw-r--r--   0        0        0     3111 2023-08-22 00:24:54.445899 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders_v3.cpython-311.pyc
--rw-r--r--   0        0        0     1867 2023-09-05 04:34:51.361972 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders_v3.cpython-39.pyc
--rw-r--r--   0        0        0     1673 2023-08-22 00:24:54.446251 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_spread_account.cpython-311.pyc
--rw-r--r--   0        0        0     1164 2023-09-05 04:34:51.362491 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_spread_account.cpython-39.pyc
--rw-r--r--   0        0        0     2476 2023-08-22 00:24:54.446645 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/collect_treasury_funds.cpython-311.pyc
--rw-r--r--   0        0        0     1604 2023-09-05 04:34:51.363064 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/collect_treasury_funds.cpython-39.pyc
--rw-r--r--   0        0        0     2761 2023-08-22 00:24:54.447107 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/crank_event_queue.cpython-311.pyc
--rw-r--r--   0        0        0     1690 2023-09-05 04:34:51.363688 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/crank_event_queue.cpython-39.pyc
--rw-r--r--   0        0        0     2853 2023-08-22 00:24:54.448150 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/deposit.cpython-311.pyc
--rw-r--r--   0        0        0     1729 2023-09-05 04:34:51.364323 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/deposit.cpython-39.pyc
--rw-r--r--   0        0        0     2850 2023-08-22 00:24:54.448710 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_insurance_vault.cpython-311.pyc
--rw-r--r--   0        0        0     1777 2023-09-05 04:34:51.365049 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_insurance_vault.cpython-39.pyc
--rw-r--r--   0        0        0     2962 2023-08-22 00:24:54.449272 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_insurance_vault_v2.cpython-311.pyc
--rw-r--r--   0        0        0     1829 2023-09-05 04:34:51.365772 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_insurance_vault_v2.cpython-39.pyc
--rw-r--r--   0        0        0     2755 2023-08-22 00:24:54.449759 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_v2.cpython-311.pyc
--rw-r--r--   0        0        0     1695 2023-09-05 04:34:51.366383 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_v2.cpython-39.pyc
--rw-r--r--   0        0        0     2162 2023-08-22 00:24:54.450097 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/edit_delegated_pubkey.cpython-311.pyc
--rw-r--r--   0        0        0     1471 2023-09-05 04:34:51.366822 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/edit_delegated_pubkey.cpython-39.pyc
--rw-r--r--   0        0        0     1570 2023-08-22 00:24:54.450526 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/expire_series.cpython-311.pyc
--rw-r--r--   0        0        0     1102 2023-09-05 04:34:51.367288 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/expire_series.cpython-39.pyc
--rw-r--r--   0        0        0     1798 2023-08-22 00:24:54.450808 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/expire_series_override.cpython-311.pyc
--rw-r--r--   0        0        0     1247 2023-09-05 04:34:51.367724 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/expire_series_override.cpython-39.pyc
--rw-r--r--   0        0        0     4395 2023-08-22 00:24:54.451359 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_order_by_order_id.cpython-311.pyc
--rw-r--r--   0        0        0     2491 2023-09-05 04:34:51.368397 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_order_by_order_id.cpython-39.pyc
--rw-r--r--   0        0        0     4297 2023-08-22 00:24:54.451967 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_order_by_order_id_v2.cpython-311.pyc
--rw-r--r--   0        0        0     2457 2023-09-05 04:34:51.369125 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_order_by_order_id_v2.cpython-39.pyc
--rw-r--r--   0        0        0     4063 2023-08-22 00:24:54.452576 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_orders.cpython-311.pyc
--rw-r--r--   0        0        0     2305 2023-09-05 04:34:51.369909 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_orders.cpython-39.pyc
--rw-r--r--   0        0        0     3965 2023-08-22 00:24:54.453245 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_orders_v2.cpython-311.pyc
--rw-r--r--   0        0        0     2271 2023-09-05 04:34:51.370716 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_orders_v2.cpython-39.pyc
--rw-r--r--   0        0        0     2260 2023-08-22 00:24:54.453808 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/halt.cpython-311.pyc
--rw-r--r--   0        0        0     1449 2023-09-05 04:34:51.371388 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/halt.cpython-39.pyc
--rw-r--r--   0        0        0     2645 2023-08-22 00:24:54.454206 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_insurance_vault.cpython-311.pyc
--rw-r--r--   0        0        0     1713 2023-09-05 04:34:51.371958 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_insurance_vault.cpython-39.pyc
--rw-r--r--   0        0        0     2693 2023-08-22 00:24:54.454702 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_socialized_loss_account.cpython-311.pyc
--rw-r--r--   0        0        0     1759 2023-09-05 04:34:51.372698 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_socialized_loss_account.cpython-39.pyc
--rw-r--r--   0        0        0     2592 2023-08-22 00:24:54.455354 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_vault.cpython-311.pyc
--rw-r--r--   0        0        0     1665 2023-09-05 04:34:51.373450 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_vault.cpython-39.pyc
--rw-r--r--   0        0        0     2660 2023-08-22 00:24:54.456117 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_cross_margin_account.cpython-311.pyc
--rw-r--r--   0        0        0     1712 2023-09-05 04:34:51.374009 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_cross_margin_account.cpython-39.pyc
--rw-r--r--   0        0        0     2009 2023-08-22 00:24:54.456622 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_cross_margin_account_manager.cpython-311.pyc
--rw-r--r--   0        0        0     1374 2023-09-05 04:34:51.374569 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_cross_margin_account_manager.cpython-39.pyc
--rw-r--r--   0        0        0     2562 2023-08-22 00:24:54.457021 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_insurance_deposit_account.cpython-311.pyc
--rw-r--r--   0        0        0     1686 2023-09-05 04:34:51.375021 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_insurance_deposit_account.cpython-39.pyc
--rw-r--r--   0        0        0     2054 2023-08-22 00:24:54.457387 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_margin_account.cpython-311.pyc
--rw-r--r--   0        0        0     1357 2023-09-05 04:34:51.375477 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_margin_account.cpython-39.pyc
--rw-r--r--   0        0        0     2710 2023-08-22 00:24:54.457754 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_indexes.cpython-311.pyc
--rw-r--r--   0        0        0     1726 2023-09-05 04:34:51.375962 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_indexes.cpython-39.pyc
--rw-r--r--   0        0        0     2670 2023-08-22 00:24:54.458511 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_node.cpython-311.pyc
--rw-r--r--   0        0        0     1712 2023-09-05 04:34:51.376552 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_node.cpython-39.pyc
--rw-r--r--   0        0        0     1907 2023-08-22 00:24:54.459009 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_strikes.cpython-311.pyc
--rw-r--r--   0        0        0     1276 2023-09-05 04:34:51.377112 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_strikes.cpython-39.pyc
--rw-r--r--   0        0        0     2463 2023-08-22 00:24:54.459377 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_tif_epoch_cycle.cpython-311.pyc
--rw-r--r--   0        0        0     1591 2023-09-05 04:34:51.377580 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_tif_epoch_cycle.cpython-39.pyc
--rw-r--r--   0        0        0     2711 2023-08-22 00:24:54.459769 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders.cpython-311.pyc
--rw-r--r--   0        0        0     1636 2023-09-05 04:34:51.378174 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders.cpython-39.pyc
--rw-r--r--   0        0        0     2610 2023-08-22 00:24:54.460158 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders_v2.cpython-311.pyc
--rw-r--r--   0        0        0     1599 2023-09-05 04:34:51.378782 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders_v2.cpython-39.pyc
--rw-r--r--   0        0        0     3290 2023-08-22 00:24:54.460571 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders_v3.cpython-311.pyc
--rw-r--r--   0        0        0     1963 2023-09-05 04:34:51.379403 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders_v3.cpython-39.pyc
--rw-r--r--   0        0        0     2824 2023-08-22 00:24:54.460986 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_perp_sync_queue.cpython-311.pyc
--rw-r--r--   0        0        0     1776 2023-09-05 04:34:51.379997 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_perp_sync_queue.cpython-39.pyc
--rw-r--r--   0        0        0     1741 2023-08-22 00:24:54.461311 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_referrer_account.cpython-311.pyc
--rw-r--r--   0        0        0     1232 2023-09-05 04:34:51.380474 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_referrer_account.cpython-39.pyc
--rw-r--r--   0        0        0     2383 2023-08-22 00:24:54.461651 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_referrer_alias.cpython-311.pyc
--rw-r--r--   0        0        0     1569 2023-09-05 04:34:51.380892 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_referrer_alias.cpython-39.pyc
--rw-r--r--   0        0        0     2054 2023-08-22 00:24:54.462037 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_spread_account.cpython-311.pyc
--rw-r--r--   0        0        0     1357 2023-09-05 04:34:51.381339 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_spread_account.cpython-39.pyc
--rw-r--r--   0        0        0     2585 2023-08-22 00:24:54.462562 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_underlying.cpython-311.pyc
--rw-r--r--   0        0        0     1643 2023-09-05 04:34:51.381786 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_underlying.cpython-39.pyc
--rw-r--r--   0        0        0     2517 2023-08-22 00:24:54.463100 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_deposit_account.cpython-311.pyc
--rw-r--r--   0        0        0     1651 2023-09-05 04:34:51.382318 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_deposit_account.cpython-39.pyc
--rw-r--r--   0        0        0     2527 2023-08-22 00:24:54.463535 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_insurance_account.cpython-311.pyc
--rw-r--r--   0        0        0     1661 2023-09-05 04:34:51.382775 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_insurance_account.cpython-39.pyc
--rw-r--r--   0        0        0     2540 2023-08-22 00:24:54.463961 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_trading_fees_account.cpython-311.pyc
--rw-r--r--   0        0        0     1674 2023-09-05 04:34:51.383213 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_trading_fees_account.cpython-39.pyc
--rw-r--r--   0        0        0     4170 2023-08-22 00:24:54.464474 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_group.cpython-311.pyc
--rw-r--r--   0        0        0     2384 2023-09-05 04:34:51.383849 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_group.cpython-39.pyc
--rw-r--r--   0        0        0     4584 2023-08-22 00:24:54.465019 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_market.cpython-311.pyc
--rw-r--r--   0        0        0     2555 2023-09-05 04:34:51.384761 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_market.cpython-39.pyc
--rw-r--r--   0        0        0     2829 2023-08-22 00:24:54.465431 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_pricing.cpython-311.pyc
--rw-r--r--   0        0        0     1810 2023-09-05 04:34:51.385333 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_pricing.cpython-39.pyc
--rw-r--r--   0        0        0     2265 2023-08-22 00:24:54.465787 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_referrals_rewards_wallet.cpython-311.pyc
--rw-r--r--   0        0        0     1507 2023-09-05 04:34:51.385770 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_referrals_rewards_wallet.cpython-39.pyc
--rw-r--r--   0        0        0     3529 2023-08-22 00:24:54.466189 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_state.cpython-311.pyc
--rw-r--r--   0        0        0     2121 2023-09-05 04:34:51.386242 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_state.cpython-39.pyc
--rw-r--r--   0        0        0     2220 2023-08-22 00:24:54.466544 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_treasury_wallet.cpython-311.pyc
--rw-r--r--   0        0        0     1464 2023-09-05 04:34:51.386694 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_treasury_wallet.cpython-39.pyc
--rw-r--r--   0        0        0     2962 2023-08-22 00:24:54.466931 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/liquidate.cpython-311.pyc
--rw-r--r--   0        0        0     1776 2023-09-05 04:34:51.387270 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/liquidate.cpython-39.pyc
--rw-r--r--   0        0        0     3085 2023-08-22 00:24:54.467351 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/liquidate_v2.cpython-311.pyc
--rw-r--r--   0        0        0     1845 2023-09-05 04:34:51.387783 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/liquidate_v2.cpython-39.pyc
--rw-r--r--   0        0        0     1703 2023-08-22 00:24:54.467711 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/migrate_to_cross_margin_account.cpython-311.pyc
--rw-r--r--   0        0        0     1198 2023-09-05 04:34:51.388256 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/migrate_to_cross_margin_account.cpython-39.pyc
--rw-r--r--   0        0        0     2359 2023-08-22 00:24:54.468095 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/override_expiry.cpython-311.pyc
--rw-r--r--   0        0        0     1535 2023-09-05 04:34:51.388773 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/override_expiry.cpython-39.pyc
--rw-r--r--   0        0        0     5821 2023-08-22 00:24:54.469019 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_order.cpython-311.pyc
--rw-r--r--   0        0        0     3112 2023-09-05 04:34:51.390252 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_order.cpython-39.pyc
--rw-r--r--   0        0        0     6029 2023-08-22 00:24:54.469703 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v2.cpython-311.pyc
--rw-r--r--   0        0        0     3220 2023-09-05 04:34:51.391255 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v2.cpython-39.pyc
--rw-r--r--   0        0        0     6190 2023-08-22 00:24:54.470364 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v3.cpython-311.pyc
--rw-r--r--   0        0        0     3304 2023-09-05 04:34:51.392189 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v3.cpython-39.pyc
--rw-r--r--   0        0        0     6334 2023-08-22 00:24:54.471022 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v4.cpython-311.pyc
--rw-r--r--   0        0        0     3370 2023-09-05 04:34:51.393075 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v4.cpython-39.pyc
--rw-r--r--   0        0        0     6203 2023-08-22 00:24:54.471724 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order.cpython-311.pyc
--rw-r--r--   0        0        0     3316 2023-09-05 04:34:51.393967 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order.cpython-39.pyc
--rw-r--r--   0        0        0     6357 2023-08-22 00:24:54.472453 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order_v2.cpython-311.pyc
--rw-r--r--   0        0        0     3392 2023-09-05 04:34:51.394859 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order_v2.cpython-39.pyc
--rw-r--r--   0        0        0     6431 2023-08-22 00:24:54.473263 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order_v3.cpython-311.pyc
--rw-r--r--   0        0        0     3432 2023-09-05 04:34:51.395848 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order_v3.cpython-39.pyc
--rw-r--r--   0        0        0     3686 2023-08-22 00:24:54.473933 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/position_movement.cpython-311.pyc
--rw-r--r--   0        0        0     2206 2023-09-05 04:34:51.396658 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/position_movement.cpython-39.pyc
--rw-r--r--   0        0        0     2088 2023-08-22 00:24:54.474430 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/prune_expired_tif_orders.cpython-311.pyc
--rw-r--r--   0        0        0     1338 2023-09-05 04:34:51.397140 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/prune_expired_tif_orders.cpython-39.pyc
--rw-r--r--   0        0        0     2081 2023-08-22 00:24:54.474814 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/rebalance_insurance_vault.cpython-311.pyc
--rw-r--r--   0        0        0     1378 2023-09-05 04:34:51.397629 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/rebalance_insurance_vault.cpython-39.pyc
--rw-r--r--   0        0        0     1800 2023-08-22 00:24:54.475210 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/refer_user.cpython-311.pyc
--rw-r--r--   0        0        0     1229 2023-09-05 04:34:51.398085 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/refer_user.cpython-39.pyc
--rw-r--r--   0        0        0     1558 2023-08-22 00:24:54.475507 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/reset_num_flex_underlyings.cpython-311.pyc
--rw-r--r--   0        0        0     1123 2023-09-05 04:34:51.398415 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/reset_num_flex_underlyings.cpython-39.pyc
--rw-r--r--   0        0        0     2693 2023-08-22 00:24:54.475854 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/set_referrals_rewards.cpython-311.pyc
--rw-r--r--   0        0        0     1764 2023-09-05 04:34:51.398872 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/set_referrals_rewards.cpython-39.pyc
--rw-r--r--   0        0        0     2592 2023-08-22 00:24:54.476282 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/settle_dex_funds.cpython-311.pyc
--rw-r--r--   0        0        0     1572 2023-09-05 04:34:51.399357 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/settle_dex_funds.cpython-39.pyc
--rw-r--r--   0        0        0     2332 2023-08-22 00:24:54.476646 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/settle_positions_halted.cpython-311.pyc
--rw-r--r--   0        0        0     1521 2023-09-05 04:34:51.399905 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/settle_positions_halted.cpython-39.pyc
--rw-r--r--   0        0        0     2206 2023-08-22 00:24:54.477075 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/toggle_market_maker.cpython-311.pyc
--rw-r--r--   0        0        0     1456 2023-09-05 04:34:51.400529 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/toggle_market_maker.cpython-39.pyc
--rw-r--r--   0        0        0     1672 2023-08-22 00:24:54.477394 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/toggle_zeta_group_perps_only.cpython-311.pyc
--rw-r--r--   0        0        0     1173 2023-09-05 04:34:51.401023 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/toggle_zeta_group_perps_only.cpython-39.pyc
--rw-r--r--   0        0        0     1816 2023-08-22 00:24:54.477991 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/transfer_excess_spread_balance.cpython-311.pyc
--rw-r--r--   0        0        0     1242 2023-09-05 04:34:51.401429 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/transfer_excess_spread_balance.cpython-39.pyc
--rw-r--r--   0        0        0     2880 2023-08-22 00:24:54.478351 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/treasury_movement.cpython-311.pyc
--rw-r--r--   0        0        0     1818 2023-09-05 04:34:51.401849 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/treasury_movement.cpython-39.pyc
--rw-r--r--   0        0        0     2268 2023-08-22 00:24:54.478674 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/unhalt.cpython-311.pyc
--rw-r--r--   0        0        0     1457 2023-09-05 04:34:51.402361 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/unhalt.cpython-39.pyc
--rw-r--r--   0        0        0     1627 2023-08-22 00:24:54.478955 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_admin.cpython-311.pyc
--rw-r--r--   0        0        0     1127 2023-09-05 04:34:51.402723 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_admin.cpython-39.pyc
--rw-r--r--   0        0        0     2254 2023-08-22 00:24:54.479239 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_halt_state.cpython-311.pyc
--rw-r--r--   0        0        0     1496 2023-09-05 04:34:51.403204 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_halt_state.cpython-39.pyc
--rw-r--r--   0        0        0     2498 2023-08-22 00:24:54.479568 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_interest_rate.cpython-311.pyc
--rw-r--r--   0        0        0     1608 2023-09-05 04:34:51.403620 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_interest_rate.cpython-39.pyc
--rw-r--r--   0        0        0     2607 2023-08-22 00:24:54.479936 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_margin_parameters.cpython-311.pyc
--rw-r--r--   0        0        0     1687 2023-09-05 04:34:51.404073 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_margin_parameters.cpython-39.pyc
--rw-r--r--   0        0        0     1731 2023-08-22 00:24:54.480273 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_oracle.cpython-311.pyc
--rw-r--r--   0        0        0     1172 2023-09-05 04:34:51.404592 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_oracle.cpython-39.pyc
--rw-r--r--   0        0        0     1765 2023-08-22 00:24:54.480588 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_oracle_backup_feed.cpython-311.pyc
--rw-r--r--   0        0        0     1206 2023-09-05 04:34:51.405036 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_oracle_backup_feed.cpython-39.pyc
--rw-r--r--   0        0        0     2593 2023-08-22 00:24:54.480997 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_perp_parameters.cpython-311.pyc
--rw-r--r--   0        0        0     1673 2023-09-05 04:34:51.405583 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_perp_parameters.cpython-39.pyc
--rw-r--r--   0        0        0     2432 2023-08-22 00:24:54.481388 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_pricing_parameters.cpython-311.pyc
--rw-r--r--   0        0        0     1602 2023-09-05 04:34:51.406152 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_pricing_parameters.cpython-39.pyc
--rw-r--r--   0        0        0     2874 2023-08-22 00:24:54.481824 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_pricing_v2.cpython-311.pyc
--rw-r--r--   0        0        0     1741 2023-09-05 04:34:51.406702 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_pricing_v2.cpython-39.pyc
--rw-r--r--   0        0        0     1656 2023-08-22 00:24:54.482153 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_referrals_admin.cpython-311.pyc
--rw-r--r--   0        0        0     1156 2023-09-05 04:34:51.407185 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_referrals_admin.cpython-39.pyc
--rw-r--r--   0        0        0     1656 2023-08-22 00:24:54.482439 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_secondary_admin.cpython-311.pyc
--rw-r--r--   0        0        0     1156 2023-09-05 04:34:51.407660 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_secondary_admin.cpython-39.pyc
--rw-r--r--   0        0        0     2472 2023-08-22 00:24:54.482751 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_volatility.cpython-311.pyc
--rw-r--r--   0        0        0     1590 2023-09-05 04:34:51.408112 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_volatility.cpython-39.pyc
--rw-r--r--   0        0        0     2491 2023-08-22 00:24:54.483077 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_expiry_parameters.cpython-311.pyc
--rw-r--r--   0        0        0     1661 2023-09-05 04:34:51.408686 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_expiry_parameters.cpython-39.pyc
--rw-r--r--   0        0        0     2493 2023-08-22 00:24:54.483583 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_margin_parameters.cpython-311.pyc
--rw-r--r--   0        0        0     1663 2023-09-05 04:34:51.409158 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_margin_parameters.cpython-39.pyc
--rw-r--r--   0        0        0     2477 2023-08-22 00:24:54.483947 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_perp_parameters.cpython-311.pyc
--rw-r--r--   0        0        0     1647 2023-09-05 04:34:51.409728 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_perp_parameters.cpython-39.pyc
--rw-r--r--   0        0        0     2436 2023-08-22 00:24:54.484324 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_pricing_pubkeys.cpython-311.pyc
--rw-r--r--   0        0        0     1610 2023-09-05 04:34:51.410378 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_pricing_pubkeys.cpython-39.pyc
--rw-r--r--   0        0        0     2262 2023-08-22 00:24:54.484714 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_state.cpython-311.pyc
--rw-r--r--   0        0        0     1504 2023-09-05 04:34:51.410905 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_state.cpython-39.pyc
--rw-r--r--   0        0        0     3197 2023-08-22 00:24:54.485219 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw.cpython-311.pyc
--rw-r--r--   0        0        0     1883 2023-09-05 04:34:51.411524 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw.cpython-39.pyc
--rw-r--r--   0        0        0     2631 2023-08-22 00:24:54.485641 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_insurance_vault.cpython-311.pyc
--rw-r--r--   0        0        0     1681 2023-09-05 04:34:51.412005 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_insurance_vault.cpython-39.pyc
--rw-r--r--   0        0        0     2743 2023-08-22 00:24:54.486152 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_insurance_vault_v2.cpython-311.pyc
--rw-r--r--   0        0        0     1733 2023-09-05 04:34:51.412471 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_insurance_vault_v2.cpython-39.pyc
--rw-r--r--   0        0        0     2759 2023-08-22 00:24:54.486542 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_v2.cpython-311.pyc
--rw-r--r--   0        0        0     1699 2023-09-05 04:34:51.413104 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_v2.cpython-39.pyc
--rw-r--r--   0        0        0     1206 2023-08-21 13:18:23.310317 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/apply_perp_funding.py
--rw-r--r--   0        0        0     2796 2023-08-21 13:18:23.301463 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/cancel_all_market_orders.py
--rw-r--r--   0        0        0     2933 2023-08-21 13:18:23.308040 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/cancel_order.py
--rw-r--r--   0        0        0     2929 2023-08-21 13:18:23.220588 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/cancel_order_by_client_order_id.py
--rw-r--r--   0        0        0     2969 2023-08-21 13:18:23.251008 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/cancel_order_by_client_order_id_no_error.py
--rw-r--r--   0        0        0     2862 2023-08-21 13:18:23.240177 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/cancel_order_halted.py
--rw-r--r--   0        0        0     2964 2023-08-21 13:18:23.181610 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/cancel_order_no_error.py
--rw-r--r--   0        0        0     1482 2023-08-21 13:18:23.259403 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/claim_referrals_rewards.py
--rw-r--r--   0        0        0     1444 2023-08-21 13:18:23.213483 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/close_cross_margin_account.py
--rw-r--r--   0        0        0     1033 2023-08-21 13:18:23.186210 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/close_cross_margin_account_manager.py
--rw-r--r--   0        0        0     2108 2023-08-21 13:18:23.233687 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/close_open_orders_v3.py
--rw-r--r--   0        0        0     1769 2023-08-21 13:18:23.279199 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/crank_event_queue.py
--rw-r--r--   0        0        0     1873 2023-08-21 13:18:23.284175 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/deposit_v2.py
--rw-r--r--   0        0        0     1822 2023-08-21 13:18:23.282423 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/initialize_cross_margin_account.py
--rw-r--r--   0        0        0     1405 2023-08-21 13:18:23.180280 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/initialize_cross_margin_account_manager.py
--rw-r--r--   0        0        0     2273 2023-08-21 13:18:23.294490 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/initialize_open_orders_v3.py
--rw-r--r--   0        0        0     1071 2023-08-21 13:18:23.299119 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/initialize_referrer_account.py
--rw-r--r--   0        0        0     1453 2023-08-21 13:18:23.206662 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/initialize_referrer_alias.py
--rw-r--r--   0        0        0     1619 2023-08-21 13:18:23.215581 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/initialize_zeta_referrals_rewards_wallet.py
--rw-r--r--   0        0        0     2073 2023-08-21 13:18:23.241514 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/liquidate_v2.py
--rw-r--r--   0        0        0     5369 2023-08-21 13:18:23.189912 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/place_perp_order_v3.py
--rw-r--r--   0        0        0     6663 2023-10-06 12:44:28.864096 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/place_perp_order_v4.py
--rw-r--r--   0        0        0     1145 2023-08-21 13:18:23.306809 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/refer_user.py
--rw-r--r--   0        0        0     1884 2023-08-21 13:18:23.192376 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/withdraw_v2.py
--rw-r--r--   0        0        0      114 2023-08-13 11:19:49.575139 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/program_id.py
--rw-r--r--   0        0        0     4672 2023-08-21 13:18:23.349433 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__init__.py
--rw-r--r--   0        0        0     6644 2023-08-21 18:06:22.716125 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4889 2023-09-05 04:34:47.033130 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2599 2023-08-21 18:06:22.716920 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/anchor_decimal.cpython-311.pyc
--rw-r--r--   0        0        0     1707 2023-09-05 04:34:47.033906 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/anchor_decimal.cpython-39.pyc
--rw-r--r--   0        0        0     7787 2023-08-21 18:06:22.718036 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/asset.cpython-311.pyc
--rw-r--r--   0        0        0     5870 2023-10-24 12:26:03.646386 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/asset.cpython-39.pyc
--rw-r--r--   0        0        0     2429 2023-08-21 18:06:22.719430 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/cross_margin_account_info.cpython-311.pyc
--rw-r--r--   0        0        0     1689 2023-09-05 04:34:47.037098 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/cross_margin_account_info.cpython-39.pyc
--rw-r--r--   0        0        0     2434 2023-08-21 18:06:22.720306 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/expire_series_override_args.cpython-311.pyc
--rw-r--r--   0        0        0     1709 2023-09-05 04:34:47.038017 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/expire_series_override_args.cpython-39.pyc
--rw-r--r--   0        0        0     2694 2023-08-21 18:06:22.721034 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/expiry_series.cpython-311.pyc
--rw-r--r--   0        0        0     1809 2023-09-05 04:34:47.038895 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/expiry_series.cpython-39.pyc
--rw-r--r--   0        0        0     7568 2023-08-21 18:06:22.722530 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/expiry_series_status.cpython-311.pyc
--rw-r--r--   0        0        0     4649 2023-09-05 04:34:47.040287 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/expiry_series_status.cpython-39.pyc
--rw-r--r--   0        0        0     2317 2023-08-21 18:06:22.723597 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/halt_args.cpython-311.pyc
--rw-r--r--   0        0        0     1574 2023-09-05 04:34:47.041819 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/halt_args.cpython-39.pyc
--rw-r--r--   0        0        0     4056 2023-08-21 18:06:22.724431 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/halt_state.cpython-311.pyc
--rw-r--r--   0        0        0     2488 2023-09-05 04:34:47.042916 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/halt_state.cpython-39.pyc
--rw-r--r--   0        0        0     2842 2023-08-21 18:06:22.725472 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/halt_state_args.cpython-311.pyc
--rw-r--r--   0        0        0     1835 2023-09-05 04:34:47.044139 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/halt_state_args.cpython-39.pyc
--rw-r--r--   0        0        0     2659 2023-08-21 18:06:22.726273 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/halt_state_v2.cpython-311.pyc
--rw-r--r--   0        0        0     1782 2023-09-05 04:34:47.045256 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/halt_state_v2.cpython-39.pyc
--rw-r--r--   0        0        0     4157 2023-08-21 18:06:22.727261 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_market_args.cpython-311.pyc
--rw-r--r--   0        0        0     2557 2023-09-05 04:34:47.046294 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_market_args.cpython-39.pyc
--rw-r--r--   0        0        0     2360 2023-08-21 18:06:22.728087 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_market_node_args.cpython-311.pyc
--rw-r--r--   0        0        0     1668 2023-09-05 04:34:47.047345 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_market_node_args.cpython-39.pyc
--rw-r--r--   0        0        0     6761 2023-08-21 18:06:22.729097 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_state_args.cpython-311.pyc
--rw-r--r--   0        0        0     3526 2023-09-05 04:34:47.048650 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_state_args.cpython-39.pyc
--rw-r--r--   0        0        0     9674 2023-08-21 18:06:22.730789 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_zeta_group_args.cpython-311.pyc
--rw-r--r--   0        0        0     4880 2023-09-05 04:34:47.050451 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_zeta_group_args.cpython-39.pyc
--rw-r--r--   0        0        0     3187 2023-08-21 18:06:22.732491 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_zeta_pricing_args.cpython-311.pyc
--rw-r--r--   0        0        0     2109 2023-09-05 04:34:47.052209 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_zeta_pricing_args.cpython-39.pyc
--rw-r--r--   0        0        0     7227 2023-08-21 18:06:22.733600 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/kind.cpython-311.pyc
--rw-r--r--   0        0        0     4520 2023-09-05 04:34:47.053562 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/kind.cpython-39.pyc
--rw-r--r--   0        0        0     3874 2023-08-21 18:06:22.734843 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/margin_account_type.cpython-311.pyc
--rw-r--r--   0        0        0     2468 2023-09-05 04:34:47.054955 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/margin_account_type.cpython-39.pyc
--rw-r--r--   0        0        0     2396 2023-08-21 18:06:22.735735 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/margin_parameters.cpython-311.pyc
--rw-r--r--   0        0        0     1663 2023-09-05 04:34:47.055914 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/margin_parameters.cpython-39.pyc
--rw-r--r--   0        0        0     6497 2023-08-21 18:06:22.736784 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/margin_requirement.cpython-311.pyc
--rw-r--r--   0        0        0     4073 2023-09-05 04:34:47.057005 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/margin_requirement.cpython-39.pyc
--rw-r--r--   0        0        0     5046 2023-08-21 18:06:22.737938 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/movement_type.cpython-311.pyc
--rw-r--r--   0        0        0     3134 2023-09-05 04:34:47.058505 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/movement_type.cpython-39.pyc
--rw-r--r--   0        0        0     4847 2023-08-21 18:06:22.739062 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/order_complete_type.cpython-311.pyc
--rw-r--r--   0        0        0     3135 2023-09-05 04:34:47.059810 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/order_complete_type.cpython-39.pyc
--rw-r--r--   0        0        0     2357 2023-08-21 18:06:22.740159 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/order_state.cpython-311.pyc
--rw-r--r--   0        0        0     1606 2023-09-05 04:34:47.060931 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/order_state.cpython-39.pyc
--rw-r--r--   0        0        0     7572 2023-08-21 18:06:22.741468 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/order_type.cpython-311.pyc
--rw-r--r--   0        0        0     4651 2023-09-05 04:34:47.062053 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/order_type.cpython-39.pyc
--rw-r--r--   0        0        0     2528 2023-08-21 18:06:22.742713 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/override_expiry_args.cpython-311.pyc
--rw-r--r--   0        0        0     1735 2023-09-05 04:34:47.064126 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/override_expiry_args.cpython-39.pyc
--rw-r--r--   0        0        0     2564 2023-08-21 18:06:22.745412 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/perp_parameters.cpython-311.pyc
--rw-r--r--   0        0        0     1746 2023-09-05 04:34:47.065087 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/perp_parameters.cpython-39.pyc
--rw-r--r--   0        0        0     3911 2023-08-21 18:06:22.746421 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/place_order_type.cpython-311.pyc
--rw-r--r--   0        0        0     2494 2023-09-05 04:34:47.066055 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/place_order_type.cpython-39.pyc
--rw-r--r--   0        0        0     2286 2023-08-21 18:06:22.747352 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/position.cpython-311.pyc
--rw-r--r--   0        0        0     1551 2023-09-05 04:34:47.067011 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/position.cpython-39.pyc
--rw-r--r--   0        0        0     2323 2023-08-21 18:06:22.748216 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/position_movement_arg.cpython-311.pyc
--rw-r--r--   0        0        0     1631 2023-09-05 04:34:47.067868 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/position_movement_arg.cpython-39.pyc
--rw-r--r--   0        0        0     5240 2023-08-21 18:06:22.749349 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/pricing_parameters.cpython-311.pyc
--rw-r--r--   0        0        0     2794 2023-09-05 04:34:47.068945 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/pricing_parameters.cpython-39.pyc
--rw-r--r--   0        0        0     3558 2023-08-21 18:06:22.750368 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/product.cpython-311.pyc
--rw-r--r--   0        0        0     2129 2023-09-05 04:34:47.070256 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/product.cpython-39.pyc
--rw-r--r--   0        0        0     3257 2023-08-21 18:06:22.752004 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/product_greeks.cpython-311.pyc
--rw-r--r--   0        0        0     1940 2023-09-05 04:34:47.072147 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/product_greeks.cpython-39.pyc
--rw-r--r--   0        0        0     3135 2023-08-21 18:06:22.752848 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/product_ledger.cpython-311.pyc
--rw-r--r--   0        0        0     1892 2023-09-05 04:34:47.073051 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/product_ledger.cpython-39.pyc
--rw-r--r--   0        0        0     2906 2023-08-21 18:06:22.753666 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/set_referrals_rewards_args.cpython-311.pyc
--rw-r--r--   0        0        0     1972 2023-09-05 04:34:47.073964 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/set_referrals_rewards_args.cpython-39.pyc
--rw-r--r--   0        0        0     4825 2023-08-21 18:06:22.754710 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/side.cpython-311.pyc
--rw-r--r--   0        0        0     3109 2023-09-05 04:34:47.075048 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/side.cpython-39.pyc
--rw-r--r--   0        0        0     2232 2023-08-21 18:06:22.750944 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/strike.cpython-311.pyc
--rw-r--r--   0        0        0     1540 2023-09-05 04:34:47.070960 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/strike.cpython-39.pyc
--rw-r--r--   0        0        0     3935 2023-08-21 18:06:22.755782 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/trait_type.cpython-311.pyc
--rw-r--r--   0        0        0     2513 2023-09-05 04:34:47.076389 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/trait_type.cpython-39.pyc
--rw-r--r--   0        0        0     7564 2023-08-21 18:06:22.756952 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/treasury_movement_type.cpython-311.pyc
--rw-r--r--   0        0        0     5023 2023-09-05 04:34:47.077698 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/treasury_movement_type.cpython-39.pyc
--rw-r--r--   0        0        0     2818 2023-08-21 18:06:22.758161 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_greeks_args.cpython-311.pyc
--rw-r--r--   0        0        0     1877 2023-09-05 04:34:47.079115 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_greeks_args.cpython-39.pyc
--rw-r--r--   0        0        0     2414 2023-08-21 18:06:22.759085 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_interest_rate_args.cpython-311.pyc
--rw-r--r--   0        0        0     1672 2023-09-05 04:34:47.080076 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_interest_rate_args.cpython-39.pyc
--rw-r--r--   0        0        0     2478 2023-08-21 18:06:22.759919 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_margin_parameters_args.cpython-311.pyc
--rw-r--r--   0        0        0     1745 2023-09-05 04:34:47.080901 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_margin_parameters_args.cpython-39.pyc
--rw-r--r--   0        0        0     2651 2023-08-21 18:06:22.760740 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_perp_parameters_args.cpython-311.pyc
--rw-r--r--   0        0        0     1833 2023-09-05 04:34:47.081739 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_perp_parameters_args.cpython-39.pyc
--rw-r--r--   0        0        0     3885 2023-08-21 18:06:22.761683 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_pricing_parameters_args.cpython-311.pyc
--rw-r--r--   0        0        0     2466 2023-09-05 04:34:47.082710 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_pricing_parameters_args.cpython-39.pyc
--rw-r--r--   0        0        0     6088 2023-08-21 18:06:22.763022 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_state_args.cpython-311.pyc
--rw-r--r--   0        0        0     3238 2023-09-05 04:34:47.084084 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_state_args.cpython-39.pyc
--rw-r--r--   0        0        0     2431 2023-08-21 18:06:22.764146 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_volatility_args.cpython-311.pyc
--rw-r--r--   0        0        0     1677 2023-09-05 04:34:47.085519 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_volatility_args.cpython-39.pyc
--rw-r--r--   0        0        0     2476 2023-08-21 18:06:22.764956 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_zeta_group_expiry_args.cpython-311.pyc
--rw-r--r--   0        0        0     1745 2023-09-05 04:34:47.086748 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_zeta_group_expiry_args.cpython-39.pyc
--rw-r--r--   0        0        0     4064 2023-08-21 18:06:22.765908 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_zeta_pricing_pubkeys_args.cpython-311.pyc
--rw-r--r--   0        0        0     2437 2023-09-05 04:34:47.087772 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_zeta_pricing_pubkeys_args.cpython-39.pyc
--rw-r--r--   0        0        0     5063 2023-08-21 18:06:22.766964 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/validation_type.cpython-311.pyc
--rw-r--r--   0        0        0     3158 2023-09-05 04:34:47.088981 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/validation_type.cpython-39.pyc
--rw-r--r--   0        0        0     1038 2023-08-21 13:18:23.328958 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/anchor_decimal.py
--rw-r--r--   0        0        0     4212 2023-10-24 12:06:35.660611 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/asset.py
--rw-r--r--   0        0        0      993 2023-08-21 13:18:23.374618 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/cross_margin_account_info.py
--rw-r--r--   0        0        0     1278 2023-08-21 13:18:23.380815 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/expire_series_override_args.py
--rw-r--r--   0        0        0     1523 2023-08-21 13:18:23.341060 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/expiry_series.py
--rw-r--r--   0        0        0     3645 2023-08-21 13:18:23.363221 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/expiry_series_status.py
--rw-r--r--   0        0        0      961 2023-08-21 13:18:23.343517 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/halt_args.py
--rw-r--r--   0        0        0     4228 2023-08-21 13:18:23.376033 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/halt_state.py
--rw-r--r--   0        0        0     1393 2023-08-21 13:18:23.344546 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/halt_state_args.py
--rw-r--r--   0        0        0     1604 2023-08-21 13:18:23.322650 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/halt_state_v2.py
--rw-r--r--   0        0        0     3631 2023-08-21 13:18:23.332919 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/initialize_market_args.py
--rw-r--r--   0        0        0      930 2023-08-21 13:18:23.337540 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/initialize_market_node_args.py
--rw-r--r--   0        0        0     9402 2023-08-21 13:18:23.372325 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/initialize_state_args.py
--rw-r--r--   0        0        0    10614 2023-08-21 13:18:23.361517 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/initialize_zeta_group_args.py
--rw-r--r--   0        0        0     2779 2023-08-21 13:18:23.355022 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/initialize_zeta_pricing_args.py
--rw-r--r--   0        0        0     3320 2023-08-21 13:18:23.320516 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/kind.py
--rw-r--r--   0        0        0     1781 2023-08-21 13:18:23.342381 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/margin_account_type.py
--rw-r--r--   0        0        0     1434 2023-08-21 13:18:23.335426 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/margin_parameters.py
--rw-r--r--   0        0        0     3463 2023-08-21 13:18:23.357981 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/margin_requirement.py
--rw-r--r--   0        0        0     2248 2023-08-21 13:18:23.326305 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/movement_type.py
--rw-r--r--   0        0        0     2228 2023-08-21 13:18:23.370349 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/order_complete_type.py
--rw-r--r--   0        0        0     1131 2023-08-21 13:18:23.352454 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/order_state.py
--rw-r--r--   0        0        0     3690 2023-08-21 13:18:23.338871 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/order_type.py
--rw-r--r--   0        0        0     1378 2023-08-21 13:18:23.345568 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/override_expiry_args.py
--rw-r--r--   0        0        0     1771 2023-08-21 13:18:23.346598 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/perp_parameters.py
--rw-r--r--   0        0        0     1871 2023-08-21 13:18:23.327540 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/place_order_type.py
--rw-r--r--   0        0        0      924 2023-08-21 13:18:23.358945 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/position.py
--rw-r--r--   0        0        0      890 2023-08-21 13:18:23.350468 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/position_movement_arg.py
--rw-r--r--   0        0        0     4621 2023-08-21 13:18:23.319155 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/pricing_parameters.py
--rw-r--r--   0        0        0     1715 2023-08-21 13:18:23.365678 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/product.py
--rw-r--r--   0        0        0     1665 2023-08-21 13:18:23.339984 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/product_greeks.py
--rw-r--r--   0        0        0     1456 2023-08-21 13:18:23.366762 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/product_ledger.py
--rw-r--r--   0        0        0     1721 2023-08-21 13:18:23.336580 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/set_referrals_rewards_args.py
--rw-r--r--   0        0        0     2208 2023-08-21 13:18:23.364477 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/side.py
--rw-r--r--   0        0        0      838 2023-08-21 13:18:23.330199 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/strike.py
--rw-r--r--   0        0        0     1951 2023-08-21 13:18:23.377099 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/trait_type.py
--rw-r--r--   0        0        0     4721 2023-08-21 13:18:23.356683 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/treasury_movement_type.py
--rw-r--r--   0        0        0     1648 2023-08-21 13:18:23.321596 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/update_greeks_args.py
--rw-r--r--   0        0        0     1084 2023-08-21 13:18:23.373376 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/update_interest_rate_args.py
--rw-r--r--   0        0        0     1494 2023-08-21 13:18:23.369135 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/update_margin_parameters_args.py
--rw-r--r--   0        0        0     1886 2023-08-21 13:18:23.379598 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/update_perp_parameters_args.py
--rw-r--r--   0        0        0     3899 2023-08-21 13:18:23.353797 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/update_pricing_parameters_args.py
--rw-r--r--   0        0        0     8581 2023-08-21 13:18:23.324668 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/update_state_args.py
--rw-r--r--   0        0        0     1054 2023-08-21 13:18:23.351453 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/update_volatility_args.py
--rw-r--r--   0        0        0     1552 2023-08-21 13:18:23.331416 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/update_zeta_group_expiry_args.py
--rw-r--r--   0        0        0     2580 2023-08-21 13:18:23.378324 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/update_zeta_pricing_pubkeys_args.py
--rw-r--r--   0        0        0     2303 2023-08-21 13:18:23.367945 zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/validation_type.py
--rw-r--r--   0        0        0     2663 1970-01-01 00:00:00.000000 zetamarkets_py-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-14 01:58:30.329630 zetamarkets_py-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1782 2023-10-24 13:28:51.142402 zetamarkets_py-0.2.9/README.md
+-rw-r--r--   0        0        0     1499 2023-11-30 14:24:08.917839 zetamarkets_py-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-10-13 00:55:50.042915 zetamarkets_py-0.2.9/zetamarkets_py/__init__.py
+-rw-r--r--   0        0        0    50158 2023-11-30 14:22:38.294558 zetamarkets_py-0.2.9/zetamarkets_py/client.py
+-rw-r--r--   0        0        0    19180 2023-11-30 14:22:38.296055 zetamarkets_py-0.2.9/zetamarkets_py/constants.py
+-rw-r--r--   0        0        0     7352 2023-11-18 02:34:07.126035 zetamarkets_py-0.2.9/zetamarkets_py/events.py
+-rw-r--r--   0        0        0     4722 2023-11-30 14:22:55.932653 zetamarkets_py-0.2.9/zetamarkets_py/exchange.py
+-rw-r--r--   0        0        0   215636 2023-11-30 14:22:38.298023 zetamarkets_py-0.2.9/zetamarkets_py/idl/zeta.json
+-rw-r--r--   0        0        0    11913 2023-10-24 14:30:30.283034 zetamarkets_py-0.2.9/zetamarkets_py/market.py
+-rw-r--r--   0        0        0     6927 2023-10-24 12:30:20.973776 zetamarkets_py-0.2.9/zetamarkets_py/orderbook.py
+-rw-r--r--   0        0        0     3177 2023-10-22 02:53:08.878101 zetamarkets_py-0.2.9/zetamarkets_py/pda.py
+-rw-r--r--   0        0        0     6484 2023-11-14 13:45:38.014070 zetamarkets_py-0.2.9/zetamarkets_py/risk.py
+-rw-r--r--   0        0        0        0 2023-09-24 12:36:37.774834 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/__init__.py
+-rw-r--r--   0        0        0      168 2023-09-24 12:41:35.940107 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      220 2023-09-08 10:53:15.637267 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/__pycache__/constants.cpython-39.pyc
+-rw-r--r--   0        0        0      290 2023-09-14 06:08:29.746879 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/__pycache__/program_id.cpython-39.pyc
+-rw-r--r--   0        0        0      144 2023-09-24 12:41:27.831694 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/__init__.py
+-rw-r--r--   0        0        0      361 2023-09-24 12:41:35.940389 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4211 2023-09-07 08:41:22.879317 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/__pycache__/market.cpython-39.pyc
+-rw-r--r--   0        0        0     4269 2023-09-24 12:41:35.944154 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/__pycache__/market_state.cpython-39.pyc
+-rw-r--r--   0        0        0     2949 2023-09-14 06:08:29.750538 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/__pycache__/open_orders.cpython-39.pyc
+-rw-r--r--   0        0        0     2362 2023-09-14 06:08:29.749038 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/__pycache__/orderbook.cpython-39.pyc
+-rw-r--r--   0        0        0     2400 2023-09-14 06:08:29.751949 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/__pycache__/queue.cpython-39.pyc
+-rw-r--r--   0        0        0     5994 2023-09-24 12:40:15.782815 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/market_state.py
+-rw-r--r--   0        0        0     3605 2023-09-12 11:00:06.010934 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/open_orders.py
+-rw-r--r--   0        0        0     2509 2023-09-12 11:00:06.011239 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/orderbook.py
+-rw-r--r--   0        0        0     2284 2023-09-12 11:00:06.011458 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/queue.py
+-rw-r--r--   0        0        0      114 2023-09-12 11:00:06.011860 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/program_id.py
+-rw-r--r--   0        0        0      119 2023-09-12 11:00:06.012149 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/types/__init__.py
+-rw-r--r--   0        0        0      334 2023-09-14 06:08:29.740649 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/types/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2465 2023-09-14 06:08:29.741420 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/types/__pycache__/account_flags.cpython-39.pyc
+-rw-r--r--   0        0        0     2872 2023-09-16 07:26:20.093737 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/types/__pycache__/queue.cpython-39.pyc
+-rw-r--r--   0        0        0     5223 2023-09-24 11:48:22.348153 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/types/__pycache__/slab.cpython-39.pyc
+-rw-r--r--   0        0        0     3517 2023-09-12 11:00:06.012683 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/types/account_flags.py
+-rw-r--r--   0        0        0     2872 2023-09-14 08:14:56.146607 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/types/queue.py
+-rw-r--r--   0        0        0     5316 2023-09-24 09:10:25.609095 zetamarkets_py-0.2.9/zetamarkets_py/serum_client/types/slab.py
+-rw-r--r--   0        0        0     1474 2023-09-14 06:08:29.753679 zetamarkets_py-0.2.9/zetamarkets_py/solana_client/accounts/__pycache__/clock.cpython-39.pyc
+-rw-r--r--   0        0        0     1325 2023-09-12 11:00:06.013459 zetamarkets_py-0.2.9/zetamarkets_py/solana_client/accounts/clock.py
+-rw-r--r--   0        0        0     4508 2023-11-30 14:22:38.298750 zetamarkets_py-0.2.9/zetamarkets_py/types.py
+-rw-r--r--   0        0        0     4086 2023-10-24 12:19:55.145643 zetamarkets_py-0.2.9/zetamarkets_py/utils.py
+-rw-r--r--   0        0        0      242 2023-08-13 11:25:54.547491 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/README.md
+-rw-r--r--   0        0        0        0 2023-09-24 12:29:58.953532 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/__init__.py
+-rw-r--r--   0        0        0      178 2023-08-14 03:44:39.758195 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      167 2023-09-24 12:32:46.713703 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      358 2023-08-14 03:44:39.901255 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/__pycache__/program_id.cpython-311.pyc
+-rw-r--r--   0        0        0      289 2023-08-16 14:09:56.107760 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/__pycache__/program_id.cpython-39.pyc
+-rw-r--r--   0        0        0      186 2023-09-24 12:24:42.495690 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__init__.py
+-rw-r--r--   0        0        0     3685 2023-08-21 18:06:22.713829 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      434 2023-09-24 12:25:12.101200 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    11893 2023-08-22 22:09:31.466239 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/cross_margin_account.cpython-311.pyc
+-rw-r--r--   0        0        0     6227 2023-11-30 14:24:44.229331 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/cross_margin_account.cpython-39.pyc
+-rw-r--r--   0        0        0     6381 2023-08-22 22:10:16.308666 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/cross_margin_account_manager.cpython-311.pyc
+-rw-r--r--   0        0        0     3854 2023-09-05 04:34:47.091489 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/cross_margin_account_manager.cpython-39.pyc
+-rw-r--r--   0        0        0     4906 2023-08-22 22:09:46.139814 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/cross_open_orders_map.cpython-311.pyc
+-rw-r--r--   0        0        0     2998 2023-09-05 04:34:47.092791 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/cross_open_orders_map.cpython-39.pyc
+-rw-r--r--   0        0        0    13204 2023-08-21 18:06:22.777847 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/greeks.cpython-311.pyc
+-rw-r--r--   0        0        0     6404 2023-09-05 04:34:47.094576 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/greeks.cpython-39.pyc
+-rw-r--r--   0        0        0     4737 2023-08-21 18:06:22.779493 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/insurance_deposit_account.cpython-311.pyc
+-rw-r--r--   0        0        0     2924 2023-09-05 04:34:47.096158 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/insurance_deposit_account.cpython-39.pyc
+-rw-r--r--   0        0        0    11691 2023-08-21 18:06:22.780756 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/margin_account.cpython-311.pyc
+-rw-r--r--   0        0        0     5696 2023-09-05 04:34:47.097615 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/margin_account.cpython-39.pyc
+-rw-r--r--   0        0        0     4909 2023-08-21 18:06:22.781959 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/market_indexes.cpython-311.pyc
+-rw-r--r--   0        0        0     2959 2023-09-05 04:34:47.099022 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/market_indexes.cpython-39.pyc
+-rw-r--r--   0        0        0     5041 2023-08-21 18:06:22.782902 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/market_node.cpython-311.pyc
+-rw-r--r--   0        0        0     3017 2023-09-05 04:34:47.100154 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/market_node.cpython-39.pyc
+-rw-r--r--   0        0        0     4666 2023-08-21 18:06:22.783836 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/open_orders_map.cpython-311.pyc
+-rw-r--r--   0        0        0     2852 2023-09-05 04:34:47.101239 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/open_orders_map.cpython-39.pyc
+-rw-r--r--   0        0        0     6174 2023-08-21 18:06:22.784860 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/perp_sync_queue.cpython-311.pyc
+-rw-r--r--   0        0        0     3671 2023-09-05 04:34:47.102331 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/perp_sync_queue.cpython-39.pyc
+-rw-r--r--   0        0        0    27485 2023-08-21 18:06:22.786941 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/pricing.cpython-311.pyc
+-rw-r--r--   0        0        0    12029 2023-11-30 14:24:44.233880 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/pricing.cpython-39.pyc
+-rw-r--r--   0        0        0     5608 2023-08-21 18:06:22.788620 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/referral_account.cpython-311.pyc
+-rw-r--r--   0        0        0     3331 2023-09-05 04:34:47.106419 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/referral_account.cpython-39.pyc
+-rw-r--r--   0        0        0     5406 2023-08-21 18:06:22.789588 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/referrer_account.cpython-311.pyc
+-rw-r--r--   0        0        0     3259 2023-09-05 04:34:47.107566 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/referrer_account.cpython-39.pyc
+-rw-r--r--   0        0        0     5063 2023-08-21 18:06:22.790529 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/referrer_alias.cpython-311.pyc
+-rw-r--r--   0        0        0     3047 2023-09-05 04:34:47.108865 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/referrer_alias.cpython-39.pyc
+-rw-r--r--   0        0        0     4777 2023-08-21 18:06:22.791415 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/settlement_account.cpython-311.pyc
+-rw-r--r--   0        0        0     2905 2023-09-05 04:34:47.109971 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/settlement_account.cpython-39.pyc
+-rw-r--r--   0        0        0     4749 2023-08-21 18:06:22.792267 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/socialized_loss_account.cpython-311.pyc
+-rw-r--r--   0        0        0     2921 2023-09-05 04:34:47.111085 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/socialized_loss_account.cpython-39.pyc
+-rw-r--r--   0        0        0     8550 2023-08-21 18:06:22.793322 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/spread_account.cpython-311.pyc
+-rw-r--r--   0        0        0     4688 2023-09-05 04:34:47.112454 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/spread_account.cpython-39.pyc
+-rw-r--r--   0        0        0    14841 2023-08-21 18:06:22.794731 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/state.cpython-311.pyc
+-rw-r--r--   0        0        0     7166 2023-11-30 14:24:44.237600 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/state.cpython-39.pyc
+-rw-r--r--   0        0        0     4629 2023-08-21 18:06:22.796189 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/underlying.cpython-311.pyc
+-rw-r--r--   0        0        0     2822 2023-09-05 04:34:47.116137 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/underlying.cpython-39.pyc
+-rw-r--r--   0        0        0     4919 2023-08-21 18:06:22.797606 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_deposit_account.cpython-311.pyc
+-rw-r--r--   0        0        0     3026 2023-09-05 04:34:47.117112 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_deposit_account.cpython-39.pyc
+-rw-r--r--   0        0        0     4935 2023-08-21 18:06:22.798485 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_insurance_account.cpython-311.pyc
+-rw-r--r--   0        0        0     3042 2023-09-05 04:34:47.118173 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_insurance_account.cpython-39.pyc
+-rw-r--r--   0        0        0     4952 2023-08-21 18:06:22.799441 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_trading_fees_account.cpython-311.pyc
+-rw-r--r--   0        0        0     3059 2023-09-05 04:34:47.119209 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_trading_fees_account.cpython-39.pyc
+-rw-r--r--   0        0        0    16492 2023-08-21 18:06:22.800886 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/zeta_group.cpython-311.pyc
+-rw-r--r--   0        0        0     7405 2023-09-05 04:34:47.120985 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/zeta_group.cpython-39.pyc
+-rw-r--r--   0        0        0     8516 2023-11-30 14:22:38.299206 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/cross_margin_account.py
+-rw-r--r--   0        0        0    17452 2023-11-30 14:22:38.299765 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/pricing.py
+-rw-r--r--   0        0        0    14179 2023-11-30 14:22:38.299975 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/state.py
+-rw-r--r--   0        0        0      887 2023-09-24 12:24:44.931139 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/__init__.py
+-rw-r--r--   0        0        0     1754 2023-08-29 19:26:18.521414 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1169 2023-09-24 12:25:12.107723 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    30973 2023-08-29 18:24:52.982819 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/__pycache__/anchor.cpython-311.pyc
+-rw-r--r--   0        0        0    19297 2023-09-05 04:34:51.340870 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/__pycache__/anchor.cpython-39.pyc
+-rw-r--r--   0        0        0    88246 2023-08-29 18:24:52.989435 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/__pycache__/custom.cpython-311.pyc
+-rw-r--r--   0        0        0    55917 2023-09-05 04:34:51.346377 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/__pycache__/custom.cpython-39.pyc
+-rw-r--r--   0        0        0    16145 2023-08-21 13:18:23.450876 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/anchor.py
+-rw-r--r--   0        0        0    47202 2023-08-21 13:18:23.447398 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/custom.py
+-rw-r--r--   0        0        0     2819 2023-09-24 12:24:47.366668 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__init__.py
+-rw-r--r--   0        0        0    16417 2023-08-22 00:24:54.436216 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2723 2023-09-24 12:25:12.111529 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1560 2023-08-22 00:24:54.436812 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/add_market_indexes.cpython-311.pyc
+-rw-r--r--   0        0        0     1114 2023-09-05 04:34:51.350580 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/add_market_indexes.cpython-39.pyc
+-rw-r--r--   0        0        0     2236 2023-08-22 00:24:54.437323 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/add_perp_market_index.cpython-311.pyc
+-rw-r--r--   0        0        0     1480 2023-09-05 04:34:51.351219 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/add_perp_market_index.cpython-39.pyc
+-rw-r--r--   0        0        0     2211 2023-08-22 00:24:54.437941 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/apply_perp_funding.cpython-311.pyc
+-rw-r--r--   0        0        0     1460 2023-09-05 04:34:51.351889 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/apply_perp_funding.cpython-39.pyc
+-rw-r--r--   0        0        0     1899 2023-08-22 00:24:54.438531 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/burn_vault_tokens.cpython-311.pyc
+-rw-r--r--   0        0        0     1272 2023-09-05 04:34:51.352393 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/burn_vault_tokens.cpython-39.pyc
+-rw-r--r--   0        0        0     3631 2023-08-22 00:24:54.439068 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_all_market_orders.cpython-311.pyc
+-rw-r--r--   0        0        0     2129 2023-09-05 04:34:51.353010 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_all_market_orders.cpython-39.pyc
+-rw-r--r--   0        0        0     3888 2023-08-22 00:24:54.439608 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order.cpython-311.pyc
+-rw-r--r--   0        0        0     2233 2023-09-05 04:34:51.353844 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order.cpython-39.pyc
+-rw-r--r--   0        0        0     3787 2023-08-22 00:24:54.440148 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_by_client_order_id.cpython-311.pyc
+-rw-r--r--   0        0        0     2228 2023-09-05 04:34:51.354577 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_by_client_order_id.cpython-39.pyc
+-rw-r--r--   0        0        0     3819 2023-08-22 00:24:54.440786 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_by_client_order_id_no_error.cpython-311.pyc
+-rw-r--r--   0        0        0     2260 2023-09-05 04:34:51.355440 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_by_client_order_id_no_error.cpython-39.pyc
+-rw-r--r--   0        0        0     3802 2023-08-22 00:24:54.441360 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_halted.cpython-311.pyc
+-rw-r--r--   0        0        0     2210 2023-09-05 04:34:51.356261 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_halted.cpython-39.pyc
+-rw-r--r--   0        0        0     3920 2023-08-22 00:24:54.441941 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_no_error.cpython-311.pyc
+-rw-r--r--   0        0        0     2265 2023-09-05 04:34:51.356941 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_no_error.cpython-39.pyc
+-rw-r--r--   0        0        0     2074 2023-08-22 00:24:54.442349 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/claim_referrals_rewards.cpython-311.pyc
+-rw-r--r--   0        0        0     1377 2023-09-05 04:34:51.357533 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/claim_referrals_rewards.cpython-39.pyc
+-rw-r--r--   0        0        0     2431 2023-08-22 00:24:54.442726 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/clean_zeta_market_halted.cpython-311.pyc
+-rw-r--r--   0        0        0     1560 2023-09-05 04:34:51.358036 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/clean_zeta_market_halted.cpython-39.pyc
+-rw-r--r--   0        0        0     1546 2023-08-22 00:24:54.443264 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/clean_zeta_markets.cpython-311.pyc
+-rw-r--r--   0        0        0     1105 2023-09-05 04:34:51.358697 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/clean_zeta_markets.cpython-39.pyc
+-rw-r--r--   0        0        0     2281 2023-08-22 00:24:54.443819 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_cross_margin_account.cpython-311.pyc
+-rw-r--r--   0        0        0     1521 2023-09-05 04:34:51.359308 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_cross_margin_account.cpython-39.pyc
+-rw-r--r--   0        0        0     1628 2023-08-22 00:24:54.444234 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_cross_margin_account_manager.cpython-311.pyc
+-rw-r--r--   0        0        0     1181 2023-09-05 04:34:51.359797 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_cross_margin_account_manager.cpython-39.pyc
+-rw-r--r--   0        0        0     1673 2023-08-22 00:24:54.444537 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_margin_account.cpython-311.pyc
+-rw-r--r--   0        0        0     1164 2023-09-05 04:34:51.360201 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_margin_account.cpython-39.pyc
+-rw-r--r--   0        0        0     2849 2023-08-22 00:24:54.444993 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders.cpython-311.pyc
+-rw-r--r--   0        0        0     1721 2023-09-05 04:34:51.360793 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders.cpython-39.pyc
+-rw-r--r--   0        0        0     2750 2023-08-22 00:24:54.445492 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders_v2.cpython-311.pyc
+-rw-r--r--   0        0        0     1686 2023-09-05 04:34:51.361413 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders_v2.cpython-39.pyc
+-rw-r--r--   0        0        0     3111 2023-08-22 00:24:54.445899 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders_v3.cpython-311.pyc
+-rw-r--r--   0        0        0     1867 2023-09-05 04:34:51.361972 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders_v3.cpython-39.pyc
+-rw-r--r--   0        0        0     1673 2023-08-22 00:24:54.446251 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_spread_account.cpython-311.pyc
+-rw-r--r--   0        0        0     1164 2023-09-05 04:34:51.362491 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_spread_account.cpython-39.pyc
+-rw-r--r--   0        0        0     2476 2023-08-22 00:24:54.446645 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/collect_treasury_funds.cpython-311.pyc
+-rw-r--r--   0        0        0     1604 2023-09-05 04:34:51.363064 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/collect_treasury_funds.cpython-39.pyc
+-rw-r--r--   0        0        0     2761 2023-08-22 00:24:54.447107 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/crank_event_queue.cpython-311.pyc
+-rw-r--r--   0        0        0     1690 2023-09-05 04:34:51.363688 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/crank_event_queue.cpython-39.pyc
+-rw-r--r--   0        0        0     2853 2023-08-22 00:24:54.448150 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/deposit.cpython-311.pyc
+-rw-r--r--   0        0        0     1729 2023-09-05 04:34:51.364323 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/deposit.cpython-39.pyc
+-rw-r--r--   0        0        0     2850 2023-08-22 00:24:54.448710 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_insurance_vault.cpython-311.pyc
+-rw-r--r--   0        0        0     1777 2023-09-05 04:34:51.365049 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_insurance_vault.cpython-39.pyc
+-rw-r--r--   0        0        0     2962 2023-08-22 00:24:54.449272 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_insurance_vault_v2.cpython-311.pyc
+-rw-r--r--   0        0        0     1829 2023-09-05 04:34:51.365772 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_insurance_vault_v2.cpython-39.pyc
+-rw-r--r--   0        0        0     2755 2023-08-22 00:24:54.449759 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_v2.cpython-311.pyc
+-rw-r--r--   0        0        0     1695 2023-09-05 04:34:51.366383 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_v2.cpython-39.pyc
+-rw-r--r--   0        0        0     2162 2023-08-22 00:24:54.450097 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/edit_delegated_pubkey.cpython-311.pyc
+-rw-r--r--   0        0        0     1471 2023-09-05 04:34:51.366822 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/edit_delegated_pubkey.cpython-39.pyc
+-rw-r--r--   0        0        0     1570 2023-08-22 00:24:54.450526 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/expire_series.cpython-311.pyc
+-rw-r--r--   0        0        0     1102 2023-09-05 04:34:51.367288 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/expire_series.cpython-39.pyc
+-rw-r--r--   0        0        0     1798 2023-08-22 00:24:54.450808 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/expire_series_override.cpython-311.pyc
+-rw-r--r--   0        0        0     1247 2023-09-05 04:34:51.367724 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/expire_series_override.cpython-39.pyc
+-rw-r--r--   0        0        0     4395 2023-08-22 00:24:54.451359 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_order_by_order_id.cpython-311.pyc
+-rw-r--r--   0        0        0     2491 2023-09-05 04:34:51.368397 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_order_by_order_id.cpython-39.pyc
+-rw-r--r--   0        0        0     4297 2023-08-22 00:24:54.451967 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_order_by_order_id_v2.cpython-311.pyc
+-rw-r--r--   0        0        0     2457 2023-09-05 04:34:51.369125 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_order_by_order_id_v2.cpython-39.pyc
+-rw-r--r--   0        0        0     4063 2023-08-22 00:24:54.452576 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_orders.cpython-311.pyc
+-rw-r--r--   0        0        0     2305 2023-09-05 04:34:51.369909 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_orders.cpython-39.pyc
+-rw-r--r--   0        0        0     3965 2023-08-22 00:24:54.453245 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_orders_v2.cpython-311.pyc
+-rw-r--r--   0        0        0     2271 2023-09-05 04:34:51.370716 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_orders_v2.cpython-39.pyc
+-rw-r--r--   0        0        0     2260 2023-08-22 00:24:54.453808 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/halt.cpython-311.pyc
+-rw-r--r--   0        0        0     1449 2023-09-05 04:34:51.371388 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/halt.cpython-39.pyc
+-rw-r--r--   0        0        0     2645 2023-08-22 00:24:54.454206 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_insurance_vault.cpython-311.pyc
+-rw-r--r--   0        0        0     1713 2023-09-05 04:34:51.371958 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_insurance_vault.cpython-39.pyc
+-rw-r--r--   0        0        0     2693 2023-08-22 00:24:54.454702 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_socialized_loss_account.cpython-311.pyc
+-rw-r--r--   0        0        0     1759 2023-09-05 04:34:51.372698 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_socialized_loss_account.cpython-39.pyc
+-rw-r--r--   0        0        0     2592 2023-08-22 00:24:54.455354 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_vault.cpython-311.pyc
+-rw-r--r--   0        0        0     1665 2023-09-05 04:34:51.373450 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_vault.cpython-39.pyc
+-rw-r--r--   0        0        0     2660 2023-08-22 00:24:54.456117 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_cross_margin_account.cpython-311.pyc
+-rw-r--r--   0        0        0     1712 2023-09-05 04:34:51.374009 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_cross_margin_account.cpython-39.pyc
+-rw-r--r--   0        0        0     2009 2023-08-22 00:24:54.456622 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_cross_margin_account_manager.cpython-311.pyc
+-rw-r--r--   0        0        0     1374 2023-09-05 04:34:51.374569 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_cross_margin_account_manager.cpython-39.pyc
+-rw-r--r--   0        0        0     2562 2023-08-22 00:24:54.457021 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_insurance_deposit_account.cpython-311.pyc
+-rw-r--r--   0        0        0     1686 2023-09-05 04:34:51.375021 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_insurance_deposit_account.cpython-39.pyc
+-rw-r--r--   0        0        0     2054 2023-08-22 00:24:54.457387 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_margin_account.cpython-311.pyc
+-rw-r--r--   0        0        0     1357 2023-09-05 04:34:51.375477 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_margin_account.cpython-39.pyc
+-rw-r--r--   0        0        0     2710 2023-08-22 00:24:54.457754 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_indexes.cpython-311.pyc
+-rw-r--r--   0        0        0     1726 2023-09-05 04:34:51.375962 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_indexes.cpython-39.pyc
+-rw-r--r--   0        0        0     2670 2023-08-22 00:24:54.458511 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_node.cpython-311.pyc
+-rw-r--r--   0        0        0     1712 2023-09-05 04:34:51.376552 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_node.cpython-39.pyc
+-rw-r--r--   0        0        0     1907 2023-08-22 00:24:54.459009 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_strikes.cpython-311.pyc
+-rw-r--r--   0        0        0     1276 2023-09-05 04:34:51.377112 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_strikes.cpython-39.pyc
+-rw-r--r--   0        0        0     2463 2023-08-22 00:24:54.459377 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_tif_epoch_cycle.cpython-311.pyc
+-rw-r--r--   0        0        0     1591 2023-09-05 04:34:51.377580 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_tif_epoch_cycle.cpython-39.pyc
+-rw-r--r--   0        0        0     2711 2023-08-22 00:24:54.459769 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders.cpython-311.pyc
+-rw-r--r--   0        0        0     1636 2023-09-05 04:34:51.378174 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders.cpython-39.pyc
+-rw-r--r--   0        0        0     2610 2023-08-22 00:24:54.460158 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders_v2.cpython-311.pyc
+-rw-r--r--   0        0        0     1599 2023-09-05 04:34:51.378782 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders_v2.cpython-39.pyc
+-rw-r--r--   0        0        0     3290 2023-08-22 00:24:54.460571 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders_v3.cpython-311.pyc
+-rw-r--r--   0        0        0     1963 2023-09-05 04:34:51.379403 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders_v3.cpython-39.pyc
+-rw-r--r--   0        0        0     2824 2023-08-22 00:24:54.460986 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_perp_sync_queue.cpython-311.pyc
+-rw-r--r--   0        0        0     1776 2023-09-05 04:34:51.379997 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_perp_sync_queue.cpython-39.pyc
+-rw-r--r--   0        0        0     1741 2023-08-22 00:24:54.461311 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_referrer_account.cpython-311.pyc
+-rw-r--r--   0        0        0     1232 2023-09-05 04:34:51.380474 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_referrer_account.cpython-39.pyc
+-rw-r--r--   0        0        0     2383 2023-08-22 00:24:54.461651 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_referrer_alias.cpython-311.pyc
+-rw-r--r--   0        0        0     1569 2023-09-05 04:34:51.380892 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_referrer_alias.cpython-39.pyc
+-rw-r--r--   0        0        0     2054 2023-08-22 00:24:54.462037 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_spread_account.cpython-311.pyc
+-rw-r--r--   0        0        0     1357 2023-09-05 04:34:51.381339 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_spread_account.cpython-39.pyc
+-rw-r--r--   0        0        0     2585 2023-08-22 00:24:54.462562 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_underlying.cpython-311.pyc
+-rw-r--r--   0        0        0     1643 2023-09-05 04:34:51.381786 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_underlying.cpython-39.pyc
+-rw-r--r--   0        0        0     2517 2023-08-22 00:24:54.463100 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_deposit_account.cpython-311.pyc
+-rw-r--r--   0        0        0     1651 2023-09-05 04:34:51.382318 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_deposit_account.cpython-39.pyc
+-rw-r--r--   0        0        0     2527 2023-08-22 00:24:54.463535 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_insurance_account.cpython-311.pyc
+-rw-r--r--   0        0        0     1661 2023-09-05 04:34:51.382775 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_insurance_account.cpython-39.pyc
+-rw-r--r--   0        0        0     2540 2023-08-22 00:24:54.463961 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_trading_fees_account.cpython-311.pyc
+-rw-r--r--   0        0        0     1674 2023-09-05 04:34:51.383213 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_trading_fees_account.cpython-39.pyc
+-rw-r--r--   0        0        0     4170 2023-08-22 00:24:54.464474 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_group.cpython-311.pyc
+-rw-r--r--   0        0        0     2384 2023-09-05 04:34:51.383849 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_group.cpython-39.pyc
+-rw-r--r--   0        0        0     4584 2023-08-22 00:24:54.465019 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_market.cpython-311.pyc
+-rw-r--r--   0        0        0     2555 2023-09-05 04:34:51.384761 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_market.cpython-39.pyc
+-rw-r--r--   0        0        0     2829 2023-08-22 00:24:54.465431 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_pricing.cpython-311.pyc
+-rw-r--r--   0        0        0     1810 2023-09-05 04:34:51.385333 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_pricing.cpython-39.pyc
+-rw-r--r--   0        0        0     2265 2023-08-22 00:24:54.465787 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_referrals_rewards_wallet.cpython-311.pyc
+-rw-r--r--   0        0        0     1507 2023-09-05 04:34:51.385770 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_referrals_rewards_wallet.cpython-39.pyc
+-rw-r--r--   0        0        0     3529 2023-08-22 00:24:54.466189 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_state.cpython-311.pyc
+-rw-r--r--   0        0        0     2121 2023-09-05 04:34:51.386242 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_state.cpython-39.pyc
+-rw-r--r--   0        0        0     2220 2023-08-22 00:24:54.466544 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_treasury_wallet.cpython-311.pyc
+-rw-r--r--   0        0        0     1464 2023-09-05 04:34:51.386694 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_treasury_wallet.cpython-39.pyc
+-rw-r--r--   0        0        0     2962 2023-08-22 00:24:54.466931 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/liquidate.cpython-311.pyc
+-rw-r--r--   0        0        0     1776 2023-09-05 04:34:51.387270 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/liquidate.cpython-39.pyc
+-rw-r--r--   0        0        0     3085 2023-08-22 00:24:54.467351 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/liquidate_v2.cpython-311.pyc
+-rw-r--r--   0        0        0     1845 2023-09-05 04:34:51.387783 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/liquidate_v2.cpython-39.pyc
+-rw-r--r--   0        0        0     1703 2023-08-22 00:24:54.467711 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/migrate_to_cross_margin_account.cpython-311.pyc
+-rw-r--r--   0        0        0     1198 2023-09-05 04:34:51.388256 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/migrate_to_cross_margin_account.cpython-39.pyc
+-rw-r--r--   0        0        0     2359 2023-08-22 00:24:54.468095 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/override_expiry.cpython-311.pyc
+-rw-r--r--   0        0        0     1535 2023-09-05 04:34:51.388773 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/override_expiry.cpython-39.pyc
+-rw-r--r--   0        0        0     5821 2023-08-22 00:24:54.469019 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_order.cpython-311.pyc
+-rw-r--r--   0        0        0     3112 2023-09-05 04:34:51.390252 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_order.cpython-39.pyc
+-rw-r--r--   0        0        0     6029 2023-08-22 00:24:54.469703 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v2.cpython-311.pyc
+-rw-r--r--   0        0        0     3220 2023-09-05 04:34:51.391255 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v2.cpython-39.pyc
+-rw-r--r--   0        0        0     6190 2023-08-22 00:24:54.470364 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v3.cpython-311.pyc
+-rw-r--r--   0        0        0     3304 2023-09-05 04:34:51.392189 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v3.cpython-39.pyc
+-rw-r--r--   0        0        0     6334 2023-08-22 00:24:54.471022 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v4.cpython-311.pyc
+-rw-r--r--   0        0        0     3370 2023-09-05 04:34:51.393075 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v4.cpython-39.pyc
+-rw-r--r--   0        0        0     6203 2023-08-22 00:24:54.471724 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order.cpython-311.pyc
+-rw-r--r--   0        0        0     3316 2023-09-05 04:34:51.393967 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order.cpython-39.pyc
+-rw-r--r--   0        0        0     6357 2023-08-22 00:24:54.472453 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order_v2.cpython-311.pyc
+-rw-r--r--   0        0        0     3392 2023-09-05 04:34:51.394859 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order_v2.cpython-39.pyc
+-rw-r--r--   0        0        0     6431 2023-08-22 00:24:54.473263 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order_v3.cpython-311.pyc
+-rw-r--r--   0        0        0     3432 2023-09-05 04:34:51.395848 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order_v3.cpython-39.pyc
+-rw-r--r--   0        0        0     3686 2023-08-22 00:24:54.473933 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/position_movement.cpython-311.pyc
+-rw-r--r--   0        0        0     2206 2023-09-05 04:34:51.396658 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/position_movement.cpython-39.pyc
+-rw-r--r--   0        0        0     2088 2023-08-22 00:24:54.474430 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/prune_expired_tif_orders.cpython-311.pyc
+-rw-r--r--   0        0        0     1338 2023-09-05 04:34:51.397140 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/prune_expired_tif_orders.cpython-39.pyc
+-rw-r--r--   0        0        0     2081 2023-08-22 00:24:54.474814 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/rebalance_insurance_vault.cpython-311.pyc
+-rw-r--r--   0        0        0     1378 2023-09-05 04:34:51.397629 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/rebalance_insurance_vault.cpython-39.pyc
+-rw-r--r--   0        0        0     1800 2023-08-22 00:24:54.475210 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/refer_user.cpython-311.pyc
+-rw-r--r--   0        0        0     1229 2023-09-05 04:34:51.398085 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/refer_user.cpython-39.pyc
+-rw-r--r--   0        0        0     1558 2023-08-22 00:24:54.475507 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/reset_num_flex_underlyings.cpython-311.pyc
+-rw-r--r--   0        0        0     1123 2023-09-05 04:34:51.398415 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/reset_num_flex_underlyings.cpython-39.pyc
+-rw-r--r--   0        0        0     2693 2023-08-22 00:24:54.475854 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/set_referrals_rewards.cpython-311.pyc
+-rw-r--r--   0        0        0     1764 2023-09-05 04:34:51.398872 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/set_referrals_rewards.cpython-39.pyc
+-rw-r--r--   0        0        0     2592 2023-08-22 00:24:54.476282 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/settle_dex_funds.cpython-311.pyc
+-rw-r--r--   0        0        0     1572 2023-09-05 04:34:51.399357 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/settle_dex_funds.cpython-39.pyc
+-rw-r--r--   0        0        0     2332 2023-08-22 00:24:54.476646 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/settle_positions_halted.cpython-311.pyc
+-rw-r--r--   0        0        0     1521 2023-09-05 04:34:51.399905 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/settle_positions_halted.cpython-39.pyc
+-rw-r--r--   0        0        0     2206 2023-08-22 00:24:54.477075 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/toggle_market_maker.cpython-311.pyc
+-rw-r--r--   0        0        0     1456 2023-09-05 04:34:51.400529 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/toggle_market_maker.cpython-39.pyc
+-rw-r--r--   0        0        0     1672 2023-08-22 00:24:54.477394 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/toggle_zeta_group_perps_only.cpython-311.pyc
+-rw-r--r--   0        0        0     1173 2023-09-05 04:34:51.401023 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/toggle_zeta_group_perps_only.cpython-39.pyc
+-rw-r--r--   0        0        0     1816 2023-08-22 00:24:54.477991 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/transfer_excess_spread_balance.cpython-311.pyc
+-rw-r--r--   0        0        0     1242 2023-09-05 04:34:51.401429 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/transfer_excess_spread_balance.cpython-39.pyc
+-rw-r--r--   0        0        0     2880 2023-08-22 00:24:54.478351 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/treasury_movement.cpython-311.pyc
+-rw-r--r--   0        0        0     1818 2023-09-05 04:34:51.401849 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/treasury_movement.cpython-39.pyc
+-rw-r--r--   0        0        0     2268 2023-08-22 00:24:54.478674 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/unhalt.cpython-311.pyc
+-rw-r--r--   0        0        0     1457 2023-09-05 04:34:51.402361 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/unhalt.cpython-39.pyc
+-rw-r--r--   0        0        0     1627 2023-08-22 00:24:54.478955 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_admin.cpython-311.pyc
+-rw-r--r--   0        0        0     1127 2023-09-05 04:34:51.402723 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_admin.cpython-39.pyc
+-rw-r--r--   0        0        0     2254 2023-08-22 00:24:54.479239 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_halt_state.cpython-311.pyc
+-rw-r--r--   0        0        0     1496 2023-09-05 04:34:51.403204 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_halt_state.cpython-39.pyc
+-rw-r--r--   0        0        0     2498 2023-08-22 00:24:54.479568 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_interest_rate.cpython-311.pyc
+-rw-r--r--   0        0        0     1608 2023-09-05 04:34:51.403620 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_interest_rate.cpython-39.pyc
+-rw-r--r--   0        0        0     2607 2023-08-22 00:24:54.479936 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_margin_parameters.cpython-311.pyc
+-rw-r--r--   0        0        0     1687 2023-09-05 04:34:51.404073 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_margin_parameters.cpython-39.pyc
+-rw-r--r--   0        0        0     1731 2023-08-22 00:24:54.480273 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_oracle.cpython-311.pyc
+-rw-r--r--   0        0        0     1172 2023-09-05 04:34:51.404592 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_oracle.cpython-39.pyc
+-rw-r--r--   0        0        0     1765 2023-08-22 00:24:54.480588 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_oracle_backup_feed.cpython-311.pyc
+-rw-r--r--   0        0        0     1206 2023-09-05 04:34:51.405036 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_oracle_backup_feed.cpython-39.pyc
+-rw-r--r--   0        0        0     2593 2023-08-22 00:24:54.480997 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_perp_parameters.cpython-311.pyc
+-rw-r--r--   0        0        0     1673 2023-09-05 04:34:51.405583 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_perp_parameters.cpython-39.pyc
+-rw-r--r--   0        0        0     2432 2023-08-22 00:24:54.481388 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_pricing_parameters.cpython-311.pyc
+-rw-r--r--   0        0        0     1602 2023-09-05 04:34:51.406152 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_pricing_parameters.cpython-39.pyc
+-rw-r--r--   0        0        0     2874 2023-08-22 00:24:54.481824 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_pricing_v2.cpython-311.pyc
+-rw-r--r--   0        0        0     1741 2023-09-05 04:34:51.406702 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_pricing_v2.cpython-39.pyc
+-rw-r--r--   0        0        0     1656 2023-08-22 00:24:54.482153 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_referrals_admin.cpython-311.pyc
+-rw-r--r--   0        0        0     1156 2023-09-05 04:34:51.407185 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_referrals_admin.cpython-39.pyc
+-rw-r--r--   0        0        0     1656 2023-08-22 00:24:54.482439 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_secondary_admin.cpython-311.pyc
+-rw-r--r--   0        0        0     1156 2023-09-05 04:34:51.407660 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_secondary_admin.cpython-39.pyc
+-rw-r--r--   0        0        0     2472 2023-08-22 00:24:54.482751 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_volatility.cpython-311.pyc
+-rw-r--r--   0        0        0     1590 2023-09-05 04:34:51.408112 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_volatility.cpython-39.pyc
+-rw-r--r--   0        0        0     2491 2023-08-22 00:24:54.483077 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_expiry_parameters.cpython-311.pyc
+-rw-r--r--   0        0        0     1661 2023-09-05 04:34:51.408686 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_expiry_parameters.cpython-39.pyc
+-rw-r--r--   0        0        0     2493 2023-08-22 00:24:54.483583 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_margin_parameters.cpython-311.pyc
+-rw-r--r--   0        0        0     1663 2023-09-05 04:34:51.409158 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_margin_parameters.cpython-39.pyc
+-rw-r--r--   0        0        0     2477 2023-08-22 00:24:54.483947 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_perp_parameters.cpython-311.pyc
+-rw-r--r--   0        0        0     1647 2023-09-05 04:34:51.409728 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_perp_parameters.cpython-39.pyc
+-rw-r--r--   0        0        0     2436 2023-08-22 00:24:54.484324 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_pricing_pubkeys.cpython-311.pyc
+-rw-r--r--   0        0        0     1610 2023-09-05 04:34:51.410378 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_pricing_pubkeys.cpython-39.pyc
+-rw-r--r--   0        0        0     2262 2023-08-22 00:24:54.484714 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_state.cpython-311.pyc
+-rw-r--r--   0        0        0     1504 2023-09-05 04:34:51.410905 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_state.cpython-39.pyc
+-rw-r--r--   0        0        0     3197 2023-08-22 00:24:54.485219 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw.cpython-311.pyc
+-rw-r--r--   0        0        0     1883 2023-09-05 04:34:51.411524 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw.cpython-39.pyc
+-rw-r--r--   0        0        0     2631 2023-08-22 00:24:54.485641 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_insurance_vault.cpython-311.pyc
+-rw-r--r--   0        0        0     1681 2023-09-05 04:34:51.412005 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_insurance_vault.cpython-39.pyc
+-rw-r--r--   0        0        0     2743 2023-08-22 00:24:54.486152 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_insurance_vault_v2.cpython-311.pyc
+-rw-r--r--   0        0        0     1733 2023-09-05 04:34:51.412471 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_insurance_vault_v2.cpython-39.pyc
+-rw-r--r--   0        0        0     2759 2023-08-22 00:24:54.486542 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_v2.cpython-311.pyc
+-rw-r--r--   0        0        0     1699 2023-09-05 04:34:51.413104 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_v2.cpython-39.pyc
+-rw-r--r--   0        0        0     1206 2023-08-21 13:18:23.310317 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/apply_perp_funding.py
+-rw-r--r--   0        0        0     2796 2023-08-21 13:18:23.301463 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/cancel_all_market_orders.py
+-rw-r--r--   0        0        0     2933 2023-08-21 13:18:23.308040 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/cancel_order.py
+-rw-r--r--   0        0        0     2929 2023-08-21 13:18:23.220588 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/cancel_order_by_client_order_id.py
+-rw-r--r--   0        0        0     2969 2023-08-21 13:18:23.251008 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/cancel_order_by_client_order_id_no_error.py
+-rw-r--r--   0        0        0     2862 2023-08-21 13:18:23.240177 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/cancel_order_halted.py
+-rw-r--r--   0        0        0     2964 2023-08-21 13:18:23.181610 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/cancel_order_no_error.py
+-rw-r--r--   0        0        0     1482 2023-08-21 13:18:23.259403 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/claim_referrals_rewards.py
+-rw-r--r--   0        0        0     1444 2023-08-21 13:18:23.213483 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/close_cross_margin_account.py
+-rw-r--r--   0        0        0     1033 2023-08-21 13:18:23.186210 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/close_cross_margin_account_manager.py
+-rw-r--r--   0        0        0     2108 2023-08-21 13:18:23.233687 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/close_open_orders_v3.py
+-rw-r--r--   0        0        0     1769 2023-08-21 13:18:23.279199 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/crank_event_queue.py
+-rw-r--r--   0        0        0     1873 2023-08-21 13:18:23.284175 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/deposit_v2.py
+-rw-r--r--   0        0        0     1822 2023-08-21 13:18:23.282423 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/initialize_cross_margin_account.py
+-rw-r--r--   0        0        0     1405 2023-08-21 13:18:23.180280 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/initialize_cross_margin_account_manager.py
+-rw-r--r--   0        0        0     2273 2023-08-21 13:18:23.294490 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/initialize_open_orders_v3.py
+-rw-r--r--   0        0        0     1071 2023-08-21 13:18:23.299119 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/initialize_referrer_account.py
+-rw-r--r--   0        0        0     1453 2023-08-21 13:18:23.206662 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/initialize_referrer_alias.py
+-rw-r--r--   0        0        0     1619 2023-08-21 13:18:23.215581 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/initialize_zeta_referrals_rewards_wallet.py
+-rw-r--r--   0        0        0     2073 2023-08-21 13:18:23.241514 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/liquidate_v2.py
+-rw-r--r--   0        0        0     5369 2023-08-21 13:18:23.189912 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/place_perp_order_v3.py
+-rw-r--r--   0        0        0     6663 2023-10-06 12:44:28.864096 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/place_perp_order_v4.py
+-rw-r--r--   0        0        0     1145 2023-08-21 13:18:23.306809 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/refer_user.py
+-rw-r--r--   0        0        0     1884 2023-08-21 13:18:23.192376 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/withdraw_v2.py
+-rw-r--r--   0        0        0      114 2023-08-13 11:19:49.575139 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/program_id.py
+-rw-r--r--   0        0        0     3510 2023-11-30 14:22:38.300166 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__init__.py
+-rw-r--r--   0        0        0     6644 2023-08-21 18:06:22.716125 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3794 2023-11-30 14:24:44.155506 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2599 2023-08-21 18:06:22.716920 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/anchor_decimal.cpython-311.pyc
+-rw-r--r--   0        0        0     1707 2023-09-05 04:34:47.033906 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/anchor_decimal.cpython-39.pyc
+-rw-r--r--   0        0        0     7787 2023-08-21 18:06:22.718036 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/asset.cpython-311.pyc
+-rw-r--r--   0        0        0     6564 2023-11-30 14:24:44.158552 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/asset.cpython-39.pyc
+-rw-r--r--   0        0        0     2429 2023-08-21 18:06:22.719430 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/cross_margin_account_info.cpython-311.pyc
+-rw-r--r--   0        0        0     1689 2023-09-05 04:34:47.037098 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/cross_margin_account_info.cpython-39.pyc
+-rw-r--r--   0        0        0     2434 2023-08-21 18:06:22.720306 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/expire_series_override_args.cpython-311.pyc
+-rw-r--r--   0        0        0     1709 2023-09-05 04:34:47.038017 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/expire_series_override_args.cpython-39.pyc
+-rw-r--r--   0        0        0     2694 2023-08-21 18:06:22.721034 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/expiry_series.cpython-311.pyc
+-rw-r--r--   0        0        0     1809 2023-09-05 04:34:47.038895 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/expiry_series.cpython-39.pyc
+-rw-r--r--   0        0        0     7568 2023-08-21 18:06:22.722530 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/expiry_series_status.cpython-311.pyc
+-rw-r--r--   0        0        0     4649 2023-09-05 04:34:47.040287 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/expiry_series_status.cpython-39.pyc
+-rw-r--r--   0        0        0     2317 2023-08-21 18:06:22.723597 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/halt_args.cpython-311.pyc
+-rw-r--r--   0        0        0     1588 2023-11-30 14:24:44.162276 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/halt_args.cpython-39.pyc
+-rw-r--r--   0        0        0     4056 2023-08-21 18:06:22.724431 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/halt_state.cpython-311.pyc
+-rw-r--r--   0        0        0     2488 2023-09-05 04:34:47.042916 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/halt_state.cpython-39.pyc
+-rw-r--r--   0        0        0     2842 2023-08-21 18:06:22.725472 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/halt_state_args.cpython-311.pyc
+-rw-r--r--   0        0        0     1835 2023-09-05 04:34:47.044139 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/halt_state_args.cpython-39.pyc
+-rw-r--r--   0        0        0     2659 2023-08-21 18:06:22.726273 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/halt_state_v2.cpython-311.pyc
+-rw-r--r--   0        0        0     1782 2023-09-05 04:34:47.045256 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/halt_state_v2.cpython-39.pyc
+-rw-r--r--   0        0        0     4157 2023-08-21 18:06:22.727261 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_market_args.cpython-311.pyc
+-rw-r--r--   0        0        0     2557 2023-09-05 04:34:47.046294 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_market_args.cpython-39.pyc
+-rw-r--r--   0        0        0     2360 2023-08-21 18:06:22.728087 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_market_node_args.cpython-311.pyc
+-rw-r--r--   0        0        0     1668 2023-09-05 04:34:47.047345 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_market_node_args.cpython-39.pyc
+-rw-r--r--   0        0        0     6761 2023-08-21 18:06:22.729097 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_state_args.cpython-311.pyc
+-rw-r--r--   0        0        0     3526 2023-09-05 04:34:47.048650 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_state_args.cpython-39.pyc
+-rw-r--r--   0        0        0     9674 2023-08-21 18:06:22.730789 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_zeta_group_args.cpython-311.pyc
+-rw-r--r--   0        0        0     4880 2023-09-05 04:34:47.050451 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_zeta_group_args.cpython-39.pyc
+-rw-r--r--   0        0        0     3187 2023-08-21 18:06:22.732491 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_zeta_pricing_args.cpython-311.pyc
+-rw-r--r--   0        0        0     2109 2023-09-05 04:34:47.052209 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_zeta_pricing_args.cpython-39.pyc
+-rw-r--r--   0        0        0     7227 2023-08-21 18:06:22.733600 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/kind.cpython-311.pyc
+-rw-r--r--   0        0        0     4520 2023-09-05 04:34:47.053562 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/kind.cpython-39.pyc
+-rw-r--r--   0        0        0     3874 2023-08-21 18:06:22.734843 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/margin_account_type.cpython-311.pyc
+-rw-r--r--   0        0        0     2468 2023-09-05 04:34:47.054955 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/margin_account_type.cpython-39.pyc
+-rw-r--r--   0        0        0     2396 2023-08-21 18:06:22.735735 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/margin_parameters.cpython-311.pyc
+-rw-r--r--   0        0        0     1663 2023-09-05 04:34:47.055914 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/margin_parameters.cpython-39.pyc
+-rw-r--r--   0        0        0     6497 2023-08-21 18:06:22.736784 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/margin_requirement.cpython-311.pyc
+-rw-r--r--   0        0        0     4073 2023-09-05 04:34:47.057005 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/margin_requirement.cpython-39.pyc
+-rw-r--r--   0        0        0     5046 2023-08-21 18:06:22.737938 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/movement_type.cpython-311.pyc
+-rw-r--r--   0        0        0     3134 2023-09-05 04:34:47.058505 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/movement_type.cpython-39.pyc
+-rw-r--r--   0        0        0     4847 2023-08-21 18:06:22.739062 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/order_complete_type.cpython-311.pyc
+-rw-r--r--   0        0        0     3135 2023-09-05 04:34:47.059810 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/order_complete_type.cpython-39.pyc
+-rw-r--r--   0        0        0     2357 2023-08-21 18:06:22.740159 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/order_state.cpython-311.pyc
+-rw-r--r--   0        0        0     1606 2023-09-05 04:34:47.060931 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/order_state.cpython-39.pyc
+-rw-r--r--   0        0        0     7572 2023-08-21 18:06:22.741468 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/order_type.cpython-311.pyc
+-rw-r--r--   0        0        0     4651 2023-09-05 04:34:47.062053 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/order_type.cpython-39.pyc
+-rw-r--r--   0        0        0     2528 2023-08-21 18:06:22.742713 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/override_expiry_args.cpython-311.pyc
+-rw-r--r--   0        0        0     1735 2023-09-05 04:34:47.064126 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/override_expiry_args.cpython-39.pyc
+-rw-r--r--   0        0        0     2564 2023-08-21 18:06:22.745412 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/perp_parameters.cpython-311.pyc
+-rw-r--r--   0        0        0     1746 2023-09-05 04:34:47.065087 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/perp_parameters.cpython-39.pyc
+-rw-r--r--   0        0        0     3911 2023-08-21 18:06:22.746421 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/place_order_type.cpython-311.pyc
+-rw-r--r--   0        0        0     2494 2023-09-05 04:34:47.066055 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/place_order_type.cpython-39.pyc
+-rw-r--r--   0        0        0     2286 2023-08-21 18:06:22.747352 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/position.cpython-311.pyc
+-rw-r--r--   0        0        0     1551 2023-09-05 04:34:47.067011 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/position.cpython-39.pyc
+-rw-r--r--   0        0        0     2323 2023-08-21 18:06:22.748216 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/position_movement_arg.cpython-311.pyc
+-rw-r--r--   0        0        0     1631 2023-09-05 04:34:47.067868 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/position_movement_arg.cpython-39.pyc
+-rw-r--r--   0        0        0     5240 2023-08-21 18:06:22.749349 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/pricing_parameters.cpython-311.pyc
+-rw-r--r--   0        0        0     2794 2023-09-05 04:34:47.068945 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/pricing_parameters.cpython-39.pyc
+-rw-r--r--   0        0        0     3558 2023-08-21 18:06:22.750368 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/product.cpython-311.pyc
+-rw-r--r--   0        0        0     2129 2023-09-05 04:34:47.070256 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/product.cpython-39.pyc
+-rw-r--r--   0        0        0     3257 2023-08-21 18:06:22.752004 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/product_greeks.cpython-311.pyc
+-rw-r--r--   0        0        0     1940 2023-09-05 04:34:47.072147 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/product_greeks.cpython-39.pyc
+-rw-r--r--   0        0        0     3135 2023-08-21 18:06:22.752848 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/product_ledger.cpython-311.pyc
+-rw-r--r--   0        0        0     1892 2023-09-05 04:34:47.073051 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/product_ledger.cpython-39.pyc
+-rw-r--r--   0        0        0     2906 2023-08-21 18:06:22.753666 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/set_referrals_rewards_args.cpython-311.pyc
+-rw-r--r--   0        0        0     1972 2023-09-05 04:34:47.073964 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/set_referrals_rewards_args.cpython-39.pyc
+-rw-r--r--   0        0        0     4825 2023-08-21 18:06:22.754710 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/side.cpython-311.pyc
+-rw-r--r--   0        0        0     3109 2023-09-05 04:34:47.075048 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/side.cpython-39.pyc
+-rw-r--r--   0        0        0     2232 2023-08-21 18:06:22.750944 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/strike.cpython-311.pyc
+-rw-r--r--   0        0        0     1540 2023-09-05 04:34:47.070960 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/strike.cpython-39.pyc
+-rw-r--r--   0        0        0     3935 2023-08-21 18:06:22.755782 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/trait_type.cpython-311.pyc
+-rw-r--r--   0        0        0     2513 2023-09-05 04:34:47.076389 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/trait_type.cpython-39.pyc
+-rw-r--r--   0        0        0     7564 2023-08-21 18:06:22.756952 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/treasury_movement_type.cpython-311.pyc
+-rw-r--r--   0        0        0     5023 2023-09-05 04:34:47.077698 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/treasury_movement_type.cpython-39.pyc
+-rw-r--r--   0        0        0     2818 2023-08-21 18:06:22.758161 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_greeks_args.cpython-311.pyc
+-rw-r--r--   0        0        0     1877 2023-09-05 04:34:47.079115 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_greeks_args.cpython-39.pyc
+-rw-r--r--   0        0        0     2414 2023-08-21 18:06:22.759085 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_interest_rate_args.cpython-311.pyc
+-rw-r--r--   0        0        0     1672 2023-09-05 04:34:47.080076 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_interest_rate_args.cpython-39.pyc
+-rw-r--r--   0        0        0     2478 2023-08-21 18:06:22.759919 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_margin_parameters_args.cpython-311.pyc
+-rw-r--r--   0        0        0     1745 2023-09-05 04:34:47.080901 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_margin_parameters_args.cpython-39.pyc
+-rw-r--r--   0        0        0     2651 2023-08-21 18:06:22.760740 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_perp_parameters_args.cpython-311.pyc
+-rw-r--r--   0        0        0     1833 2023-09-05 04:34:47.081739 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_perp_parameters_args.cpython-39.pyc
+-rw-r--r--   0        0        0     3885 2023-08-21 18:06:22.761683 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_pricing_parameters_args.cpython-311.pyc
+-rw-r--r--   0        0        0     2466 2023-09-05 04:34:47.082710 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_pricing_parameters_args.cpython-39.pyc
+-rw-r--r--   0        0        0     6088 2023-08-21 18:06:22.763022 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_state_args.cpython-311.pyc
+-rw-r--r--   0        0        0     3238 2023-09-05 04:34:47.084084 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_state_args.cpython-39.pyc
+-rw-r--r--   0        0        0     2431 2023-08-21 18:06:22.764146 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_volatility_args.cpython-311.pyc
+-rw-r--r--   0        0        0     1677 2023-09-05 04:34:47.085519 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_volatility_args.cpython-39.pyc
+-rw-r--r--   0        0        0     2476 2023-08-21 18:06:22.764956 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_zeta_group_expiry_args.cpython-311.pyc
+-rw-r--r--   0        0        0     1745 2023-09-05 04:34:47.086748 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_zeta_group_expiry_args.cpython-39.pyc
+-rw-r--r--   0        0        0     4064 2023-08-21 18:06:22.765908 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_zeta_pricing_pubkeys_args.cpython-311.pyc
+-rw-r--r--   0        0        0     2437 2023-09-05 04:34:47.087772 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_zeta_pricing_pubkeys_args.cpython-39.pyc
+-rw-r--r--   0        0        0     5063 2023-08-21 18:06:22.766964 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/validation_type.cpython-311.pyc
+-rw-r--r--   0        0        0     3158 2023-09-05 04:34:47.088981 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/validation_type.cpython-39.pyc
+-rw-r--r--   0        0        0     1038 2023-08-21 13:18:23.328958 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/anchor_decimal.py
+-rw-r--r--   0        0        0     4738 2023-11-30 14:22:38.300327 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/asset.py
+-rw-r--r--   0        0        0      993 2023-08-21 13:18:23.374618 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/cross_margin_account_info.py
+-rw-r--r--   0        0        0      961 2023-11-30 14:22:38.300464 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/halt_args.py
+-rw-r--r--   0        0        0     4228 2023-08-21 13:18:23.376033 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/halt_state.py
+-rw-r--r--   0        0        0     1393 2023-08-21 13:18:23.344546 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/halt_state_args.py
+-rw-r--r--   0        0        0     1604 2023-08-21 13:18:23.322650 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/halt_state_v2.py
+-rw-r--r--   0        0        0     3631 2023-08-21 13:18:23.332919 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/initialize_market_args.py
+-rw-r--r--   0        0        0      930 2023-08-21 13:18:23.337540 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/initialize_market_node_args.py
+-rw-r--r--   0        0        0     9402 2023-08-21 13:18:23.372325 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/initialize_state_args.py
+-rw-r--r--   0        0        0     2779 2023-08-21 13:18:23.355022 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/initialize_zeta_pricing_args.py
+-rw-r--r--   0        0        0     3320 2023-08-21 13:18:23.320516 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/kind.py
+-rw-r--r--   0        0        0     1781 2023-08-21 13:18:23.342381 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/margin_account_type.py
+-rw-r--r--   0        0        0     1434 2023-08-21 13:18:23.335426 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/margin_parameters.py
+-rw-r--r--   0        0        0     3463 2023-08-21 13:18:23.357981 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/margin_requirement.py
+-rw-r--r--   0        0        0     2248 2023-08-21 13:18:23.326305 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/movement_type.py
+-rw-r--r--   0        0        0     2228 2023-08-21 13:18:23.370349 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/order_complete_type.py
+-rw-r--r--   0        0        0     1131 2023-08-21 13:18:23.352454 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/order_state.py
+-rw-r--r--   0        0        0     3690 2023-08-21 13:18:23.338871 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/order_type.py
+-rw-r--r--   0        0        0     1771 2023-08-21 13:18:23.346598 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/perp_parameters.py
+-rw-r--r--   0        0        0     1871 2023-08-21 13:18:23.327540 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/place_order_type.py
+-rw-r--r--   0        0        0      924 2023-08-21 13:18:23.358945 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/position.py
+-rw-r--r--   0        0        0     4621 2023-08-21 13:18:23.319155 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/pricing_parameters.py
+-rw-r--r--   0        0        0     1715 2023-08-21 13:18:23.365678 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/product.py
+-rw-r--r--   0        0        0     1665 2023-08-21 13:18:23.339984 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/product_greeks.py
+-rw-r--r--   0        0        0     1456 2023-08-21 13:18:23.366762 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/product_ledger.py
+-rw-r--r--   0        0        0     1721 2023-08-21 13:18:23.336580 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/set_referrals_rewards_args.py
+-rw-r--r--   0        0        0     2208 2023-08-21 13:18:23.364477 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/side.py
+-rw-r--r--   0        0        0      838 2023-08-21 13:18:23.330199 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/strike.py
+-rw-r--r--   0        0        0     1951 2023-08-21 13:18:23.377099 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/trait_type.py
+-rw-r--r--   0        0        0     4721 2023-08-21 13:18:23.356683 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/treasury_movement_type.py
+-rw-r--r--   0        0        0     1494 2023-08-21 13:18:23.369135 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/update_margin_parameters_args.py
+-rw-r--r--   0        0        0     1886 2023-08-21 13:18:23.379598 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/update_perp_parameters_args.py
+-rw-r--r--   0        0        0     3899 2023-08-21 13:18:23.353797 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/update_pricing_parameters_args.py
+-rw-r--r--   0        0        0     8581 2023-08-21 13:18:23.324668 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/update_state_args.py
+-rw-r--r--   0        0        0     2580 2023-08-21 13:18:23.378324 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/update_zeta_pricing_pubkeys_args.py
+-rw-r--r--   0        0        0     2303 2023-08-21 13:18:23.367945 zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/validation_type.py
+-rw-r--r--   0        0        0     2621 1970-01-01 00:00:00.000000 zetamarkets_py-0.2.9/PKG-INFO
```

### Comparing `zetamarkets_py-0.2.7/LICENSE` & `zetamarkets_py-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/README.md` & `zetamarkets_py-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/pyproject.toml` & `zetamarkets_py-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "zetamarkets_py"
-version = "0.2.7"
+version = "0.2.9"
 description = "Python SDK for Zeta Markets"
 license = "apache-2.0"
 authors = ["Tristan0x <tristan@sierra.team>"]
 readme = "README.md"
 repository = "https://github.com/zetamarkets/zetamarkets-py"
 packages = [
     { include = "zetamarkets_py" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 solana = "^0.30.2"
 solders = "^0.18.1"
-requests = "^2.31.0"
 anchorpy = "^0.18.0"
 colorlog = "^6.7.0"
 deprecated = "^1.2.14"
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/client.py` & `zetamarkets_py-0.2.9/zetamarkets_py/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -638,15 +638,17 @@
             if log_messages[i].endswith("invoke [1]"):
                 split_indices.append(i)
 
         split_log_messages = [log_messages[i:j] for i, j in zip([0] + split_indices, split_indices + [None])]
         if len(split_log_messages) > 0:
             split_log_messages = split_log_messages[1:]
 
-        if len(ix_args) != len(split_log_messages) or len(ix_names) != len(split_log_messages):
+        if not ignore_truncation and (
+            len(ix_args) != len(split_log_messages) or len(ix_names) != len(split_log_messages)
+        ):
             raise Exception("Mismatched transaction info lengths")
 
         # For each individual instruction, find the ix name and the events
         for i in range(len(split_log_messages)):
             # First log line will always be "...invoke [1]", second will be "Program log: Instruction: <ix_name>"
             ix_name = ix_names[i]
             ix_arg = ix_args[i]
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/constants.py` & `zetamarkets_py-0.2.9/zetamarkets_py/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,18 +25,20 @@
 }
 
 # These are generated flexible PDAs and aren't reflective of an spl token mint.
 FLEXIBLE_MINTS = {
     Network.DEVNET: {
         Asset.APT: Pubkey.from_string("FbfkphUHaAd7c27RqhzKBRAPX8T5AzFBH259sbGmNuvG"),
         Asset.ARB: Pubkey.from_string("w8h6r5ogLihfuWeCA1gs7boxNjzbwWeQbXMB3UATaC6"),
+        Asset.PYTH: Pubkey.from_string("5PK1Ty2ac1Un6zY11Em7qF4FAYBgUu5y8Pt8ZtbepGnF"),
     },
     Network.MAINNET: {
         Asset.APT: Pubkey.from_string("8z8oShLky1PauW9hxv6AsjnricLqoK9MfmNZJDQNNNPr"),
         Asset.ARB: Pubkey.from_string("Ebd7aUFu3rtsZruCzTnG4tjBoxaJdWT8S3t4yC8hVpbo"),
+        Asset.PYTH: Pubkey.from_string("BjZmtqBVKY1oUSUjgq9PBQWJPyWbcWTXYbQ1oWxa9NYp"),
     },
 }
 
 USDC_MINT = {
     #   Network.LOCALNET: Pubkey.from_string("6PEh8n3p7BbCTykufbq1nSJYAZvUp6gSwEANAs1ZhsCX"),
     Network.DEVNET: Pubkey.from_string("6PEh8n3p7BbCTykufbq1nSJYAZvUp6gSwEANAs1ZhsCX"),
     Network.MAINNET: Pubkey.from_string("EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v"),
@@ -85,15 +87,15 @@
 QUOTE_MINT_DECIMALS = 6
 
 BLOCKHASH_COMMITMENT = commitment.Finalized
 
 ZETA_LUT = {
     # Network.LOCALNET: None,
     Network.DEVNET: AddressLookupTableAccount(
-        key=Pubkey.from_string("3a2We1NeafvL9Hnx41ZXZQRjxLxr8M6MnjneZZjJDRfZ"),
+        key=Pubkey.from_string("2ea7yKr6Z86SVrhmnujBHGuiWnxFPb6YjzM3SG2FNhW4"),
         addresses=[
             Pubkey.from_string("9VddCF6iEyZbjkCQ4g8VJpjEtuLsgmvRCc6LQwAvXigC"),
             Pubkey.from_string("BditorsEXbVw6R8Woe6JhoyXC1beJCixYt57UMKuiwQi"),
             Pubkey.from_string("5CmWtUihvSrJpaUrpJ3H1jUa9DRjYz4v2xs6c3EgQWMf"),
             Pubkey.from_string("TokenkegQfeZyiNwAJbNbGKPFXCWuBvf9Ss623VQ5DA"),
             Pubkey.from_string("7m134nU79ezr3b7jYSehnhto94AvSP4yexa3Wdhxff99"),
             Pubkey.from_string("SysvarRent111111111111111111111111111111111"),
@@ -104,14 +106,18 @@
             Pubkey.from_string("6PxBx93S8x3tno1TsFZwT5VqP8drrRCbCXygEXYNkFJe"),
             Pubkey.from_string("EdVCmQ9FSPcVe5YySXDPCRmc8aDQLKJ9xvYBMZPie1Vw"),
             Pubkey.from_string("669U43LNHx7LsVj95uYksnhXUfWKDsdzVqev3V4Jpw3P"),
             Pubkey.from_string("5d2QJ6u2NveZufmJ4noHja5EHs3Bv1DUMPLG5xfasSVs"),
             Pubkey.from_string("11111111111111111111111111111111"),
             Pubkey.from_string("5SSkXsEKQepHHAewytPVwdej4epN1nxgLVM84L4KXgy7"),
             Pubkey.from_string("11111111111111111111111111111111"),
+            Pubkey.from_string("GwzBgrXb4PG59zjce24SF2b9JXbLEjJJTBkmytuEZj1b"),
+            Pubkey.from_string("11111111111111111111111111111111"),
+            Pubkey.from_string("ELF78ZhSr8u4SCixA7YSpjdZHZoSNrAhcyysbavpC2kA"),
+            Pubkey.from_string("AVQutgTg4Jd4o4A4P4aYLJF3gpq7xmsE6DZqw1Eq2NvS"),
             Pubkey.from_string("JB43m9cTZVb4LcEfBA1Bf49nz4cod2Xt5i2HRAAMQvdo"),
             Pubkey.from_string("6YcgjoTUTeafyFC5C6vgFCVoM69qgpj966PhCojwiS4Z"),
             Pubkey.from_string("qjoUa8fC1DjsnwVwUCJQcVDJVYUhAnrqz3B9FSxVPAm"),
             Pubkey.from_string("5kSQn4o4S4mRR48sLZ5kijvCjnnD4NbwPqaBaQYvC6wk"),
             Pubkey.from_string("7Nm1pAysuk38D6uiU83wXfegzruqohVNwUippwSZNx71"),
             Pubkey.from_string("V6Y9bCVTTwjBDYAJ6ixMWWFK7RKZcQeUcpufZaM3DDB"),
             Pubkey.from_string("5yiNVYs4xpC26yY9K3DYTRvdFkdjBSnkyeSAA3Huf4Q2"),
@@ -159,18 +165,40 @@
             Pubkey.from_string("G3ytGgn7MzH5DpLCSBshkV4xQe1G4JBbTu7c9CCWA9U"),
             Pubkey.from_string("J5t2VsFLSXGTaA1o2qCujduJ9dnHLok9QhYUroN2fc6X"),
             Pubkey.from_string("6UEwXk5ixtC6rDJG7X2X6MLNwiAyjGZZyN6L1JG63n4H"),
             Pubkey.from_string("FkHx7byyFDGheXCcmVxdavTDteotaDJZk8DBNBm2Maeb"),
             Pubkey.from_string("zXEzviQpq8u89oAKdU7r3vHHxXpxC2547AoLzxCKSJ3"),
             Pubkey.from_string("93DGPpMR6w3gqbrbpZrChqw8vihgHibmdejB4Q1p4DbP"),
             Pubkey.from_string("Ag4cqXXAAxa9NCZcFgQuoeDkvtSbxwe6qaEfjw4aRnUH"),
+            Pubkey.from_string("2j1BJUDD9dXXzypVyjT5HXAy1e11VzjtMpGW4U7ynJXP"),
+            Pubkey.from_string("BN7EMGBdTBkJfAtuRhUWpDdewqk6RVF2CvyVku6fvH26"),
+            Pubkey.from_string("8yNLGd4fngCtsXeoVoEEE22Bicjkcuvq9GWbdHd6b6nK"),
+            Pubkey.from_string("HaAPQFP2nxinog4SDzJ8pZCv7eFNXxCxzhQrm5JrHckq"),
+            Pubkey.from_string("GQH1eMDvw9hysVFiiVRwdjWW4Pow5AjguY3U39Gnn1my"),
+            Pubkey.from_string("5xAbQKS8qdS4D5h78AusSraZDqyPjGfiDyzQNRBSgyqD"),
+            Pubkey.from_string("DwvnBtJW1x8LANmaVPgUt8F9uY9AEnXH9CM1dsBxvpd7"),
+            Pubkey.from_string("Ch4Gd1tyNhGnqRrHD112PvgevmCi5RA8br4CRESdJp9R"),
+            Pubkey.from_string("D2MvxY79gJUs1b1VmEiDTN85r8vgQDxU9Z2vE5oKVa4N"),
+            Pubkey.from_string("6KjVaBHGvFGcVzptCmqUgE6mRnLrbtssSP2nVN4SJWw8"),
+            Pubkey.from_string("DZP6WX2p8ZERhr9qHxpySt3hR77KU38KLFth1JfAhGe4"),
+            Pubkey.from_string("AVQutgTg4Jd4o4A4P4aYLJF3gpq7xmsE6DZqw1Eq2NvS"),
+            Pubkey.from_string("7pbGP7MoJZ7zpr5ngWrURjDMk3dgxdphnnURot7V2Nvs"),
+            Pubkey.from_string("6f35vNsWmky1wkiMGcXk7KUZUszaAfmBNv4tod9ZguXD"),
+            Pubkey.from_string("7edomgWHCcwR8rG349wWZDCVXba9BZxon5LcEnnx4kow"),
+            Pubkey.from_string("FJBabair8yvFbuYFaDK8Neqjof1BbWPS3wjpR17sKkst"),
+            Pubkey.from_string("C5oGeBgUREHZzHXjPbLLiBRBe6w6G91LYHjejQHAA6qL"),
+            Pubkey.from_string("8vrZSqsXrzMtR53iCrwVgh4bVh1LYANW2xQ5qZoQH3kw"),
+            Pubkey.from_string("5ub4h28b5d8Muf4Cw8JzET7BzCYe3vUALqXWedbzwuNG"),
+            Pubkey.from_string("2DWDgtCYtVvV6fpN9WHhMztt4fWgNcdpn5hGVcXWxe6Z"),
+            Pubkey.from_string("7Ty1AkSCmHpMLFNjH7xW2s2DkcMWggg3MkyYfWmwcKa5"),
+            Pubkey.from_string("DS4ThY5eeu7orkMbueVW2zwQVG8FUhBGn1dm1WyxH75P"),
         ],
     ),
     Network.MAINNET: AddressLookupTableAccount(
-        key=Pubkey.from_string("7Xjap9vrWush2kY3HV691U2R3b4CZgyafWcCDJiZ1zVR"),
+        key=Pubkey.from_string("pxSHSw1dQpf3fhffWxs9KEfbbKdHpcRYf9UYrh7u8R7"),
         addresses=[
             Pubkey.from_string("8eExPiLp47xbSDYkbuem4qnLUpbLTfZBeFuEJoh6EUr2"),
             Pubkey.from_string("BbKFezrmKD83PeVh74958MzgFAue1pZptipSNLz5ccpk"),
             Pubkey.from_string("zDEXqXEG7gAyxb1Kg9mK5fPnUdENCGKzWrM21RMdWRq"),
             Pubkey.from_string("TokenkegQfeZyiNwAJbNbGKPFXCWuBvf9Ss623VQ5DA"),
             Pubkey.from_string("AVNMK6wiGfppdQNg9WKfMRBXefDPGZFh2f3o1fRbgN8n"),
             Pubkey.from_string("SysvarRent111111111111111111111111111111111"),
@@ -181,14 +209,18 @@
             Pubkey.from_string("Cv4T27XbjVoKUYwP72NQQanvZeA7W4YF9L4EnYT9kx5o"),
             Pubkey.from_string("JBu1AL4obBcCMqKBBxhpWCNUt136ijcuMZLFvTP7iWdB"),
             Pubkey.from_string("716hFAECqotxcXcj8Hs8nr7AG6q9dBw2oX3k3M8V7uGq"),
             Pubkey.from_string("FNNvb1AFDnDVPkocEri8mWbJ1952HQZtFLuwPiUjSJQ"),
             Pubkey.from_string("11111111111111111111111111111111"),
             Pubkey.from_string("5HRrdmghsnU3i2u5StaKaydS7eq3vnKVKwXMzCNKsc4C"),
             Pubkey.from_string("11111111111111111111111111111111"),
+            Pubkey.from_string("4CkQJBxhU8EZ2UjhigbtdaPbpTe6mqf811fipYBFbSYN"),
+            Pubkey.from_string("F6rApkRBD31K6zZrwXt8aQrRKwzbZqCMH2vbMvBgftPX"),
+            Pubkey.from_string("nrYkQQQur7z8rYTST3G9GqATviK5SxTDkrqd21MW6Ue"),
+            Pubkey.from_string("11111111111111111111111111111111"),
             Pubkey.from_string("JE6d41JRokZAMUEAznV8JP4h7i6Ain6CyJrQuweRipFU"),
             Pubkey.from_string("EaNR74nCjrYyNDsuoWmq19pH76QSd1nuTzvJSr3RDQ6x"),
             Pubkey.from_string("3rjBffJkFa9zdGr9xmTVxF3y6nL6iL1pASVzym7s5FGr"),
             Pubkey.from_string("HcjrQKnbqKJuxHDLNM9LJPyxcQs237waNZXW7RwgvAps"),
             Pubkey.from_string("Ec4xsLLgLc4wM5c19ZSvazE7M9Rtk2T6RzddNcSQKYGu"),
             Pubkey.from_string("BEjGhNFnKT5weGtpBoFs5Y1mDN47Ntvag5aMV59nZRpk"),
             Pubkey.from_string("CHBUBfU3zscTNsihdK3x44TbpTza1hwcsTUaZfk751b5"),
@@ -236,10 +268,32 @@
             Pubkey.from_string("8if1NcDaif8dxM3Ct6rRTQEj9GFwukadU1MDQHqCnw9h"),
             Pubkey.from_string("GnSRgncxFbtxqZ4HmfnF6daCmgkc8tuQz9i37hUmwV5t"),
             Pubkey.from_string("6JjDgGzqzU6Az7ZmTARAvBSwBxfXsqbVG3Rc9JGU9i4L"),
             Pubkey.from_string("GQXdvh4dHvENTFi2CfVrh77aQD1Y6V7HMNYNCuvgbSuc"),
             Pubkey.from_string("EC2PCjwcuBBFHp6gpAKa3kdpLVrQxdy7kgr7p4wPy8Vw"),
             Pubkey.from_string("7j1N5UiXLFxaxFWq5tzZc5R3sjPHcF7jqfHJgAtE74q8"),
             Pubkey.from_string("Eqt3anUy8nqDvzJaNvWvqBM32Ln4UUnLkfvdd9Ztfj81"),
+            Pubkey.from_string("6C3K3LDgVeiKZ93d4TTsax6qxjmr2Hm61873aR8ykJYT"),
+            Pubkey.from_string("Ao4fdNfwP1KPUwxoKbKVZ3Jp12MiCsK8gvvxbumn75by"),
+            Pubkey.from_string("238aPEmvSnFdra3gMYz2NPSwHPPTaf5bGxaqMXMs35GE"),
+            Pubkey.from_string("5JLWHAW2fX7C2PFc2Len3kUfjYJAKLAyUhb8i9nr9cH3"),
+            Pubkey.from_string("HhcUi31CHLScAV1dpQq1suxsXpg331fETUZU1GsNgVSx"),
+            Pubkey.from_string("GNp5Q8fwD45azybdXKfuYYTHRkUh2krX9ejYuNKMFNmR"),
+            Pubkey.from_string("DZdqa3nVJmyPc2ei397Cr1TufzZiNG3G6aRrV1AZ52p7"),
+            Pubkey.from_string("5qxoTJ3N5GRNJnWuZ4E8Ak4MUB4hiPwyCrn3VMPmgsAM"),
+            Pubkey.from_string("3cU8siJiNomBZDB12qA5QoRTwUMi2ZUa6f496js2RUwf"),
+            Pubkey.from_string("5DPKMXmf9WK1C6N1MoJLWjYApiP4KR8zNf1oofevGEub"),
+            Pubkey.from_string("B6sV248kSsj6n72osn3Wcuz87JX3RFMD7FZpgwdYGQTm"),
+            Pubkey.from_string("ALYccFbb6ZPmUuiGeFC6pers4bfgpV2RtKoFiAsyQK8X"),
+            Pubkey.from_string("DCSXWke6HzdA8J6FhcxxM7mrdr4mkNhN32KjVAPtCZeG"),
+            Pubkey.from_string("8tjRWGXkCAszLS1XF5Vf7uEiGvhpggaG2aNmqcvuKUC8"),
+            Pubkey.from_string("8jU96TshKzrLqXzZbUL5privTaT6RQqV1rGeJ6EMuoYS"),
+            Pubkey.from_string("D9A4dFKehqpcyNDdeRYvA9hkUDa2RUTF7zN6vwZVnT6w"),
+            Pubkey.from_string("7cdY8U9Q5T5ktvF8VtkkZ1E7bt5mqbcQJQUw4433uEaV"),
+            Pubkey.from_string("137rR2TJ7ryu7nBxNNCeCdXqEt79jQLo4YvTzhEoAEh4"),
+            Pubkey.from_string("4LhMuCufFL4aR1UvnNQ4zP49FqmjRj4uVrJ9qE7L1GxS"),
+            Pubkey.from_string("8UxG6sugH55rMybJkVXt3Pb3pJh9ZfRQbzajHEDDezsT"),
+            Pubkey.from_string("7Pnbf6WLGpsYjbjnQN4t8wMCzdDGsx9ZAyuLd4vZmN49"),
+            Pubkey.from_string("5Q245C352ChdBGWmNbiYmFneAUiMjhnbPwUqmdHWJ8U6"),
         ],
     ),
 }
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/events.py` & `zetamarkets_py-0.2.9/zetamarkets_py/events.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/exchange.py` & `zetamarkets_py-0.2.9/zetamarkets_py/exchange.py`

 * *Files 18% similar despite different names*

```diff
@@ -136,42 +136,7 @@
         """
         Returns a list of keys from the markets dictionary.
 
         Returns:
             list[Asset]: A list of Asset objects.
         """
         return list(self.markets.keys())
-
-    # TODO: add auto priority fee
-    # TODO: add to solders
-    # def update_auto_fee(self):
-    #     account_list = []
-
-    #     # Query the most written-to accounts
-    #     # Note: getRecentPrioritizationFees() will account for global fees too if no one is writing to our accs
-    #     for market in self.markets.values():
-    #         account_list.append(market.address.perp_sync_queue_address)
-
-    #     try:
-    #         data = requests.post(
-    #             self.endpoint,
-    #             json={
-    #                 "jsonrpc": "2.0",
-    #                 "id": 1,
-    #                 "method": "getRecentPrioritizationFees",
-    #                 "params": [[account_list]],
-    #             },
-    #         )
-
-    #         fees = sorted(
-    #             [obj["prioritizationFee"] for obj in data.json()["result"]],
-    #             key=lambda x: x["slot"],
-    #             reverse=True,
-    #         )[
-    #             :20
-    #         ]  # Grab the latest 20
-
-    #         median = statistics.median(fees)
-    #         self.priority_fee = min(median, self._auto_priority_fee_upper_limit)
-    #         print(f"AutoUpdate priority fee. New fee = {self.priority_fee} microlamports per compute unit")
-    #     except Exception as e:
-    #         print(f"updateAutoFee failed {e}")
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/idl/zeta.json` & `zetamarkets_py-0.2.9/zetamarkets_py/idl/zeta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999583218060568%*

 * *Differences: {"'accounts'": "{0: {'type': {'fields': {1: {'type': {'array': {insert: [(1, 7)], delete: [1]}}}, "*

 * *               "2: {'type': {'array': {insert: [(1, 18)], delete: [1]}}}, 3: {'type': {'array': "*

 * *               "{insert: [(1, 7)], delete: [1]}}}, 4: {'type': {'array': {insert: [(1, 18)], "*

 * *               "delete: [1]}}}, 5: {'type': {'array': {insert: [(1, 7)], delete: [1]}}}, 6: "*

 * *               "{'type': {'array': {insert: [(1, 18)], delete: [1]}}}, 7: {'type': {'array': "*

 * *               "{insert: [(1,  […]*

```diff
@@ -9,260 +9,260 @@
                         "type": "u8"
                     },
                     {
                         "name": "markPrices",
                         "type": {
                             "array": [
                                 "u64",
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "markPricesPadding",
                         "type": {
                             "array": [
                                 "u64",
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "updateTimestamps",
                         "type": {
                             "array": [
                                 "u64",
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "updateTimestampsPadding",
                         "type": {
                             "array": [
                                 "u64",
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "fundingDeltas",
                         "type": {
                             "array": [
                                 {
                                     "defined": "AnchorDecimal"
                                 },
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "fundingDeltasPadding",
                         "type": {
                             "array": [
                                 {
                                     "defined": "AnchorDecimal"
                                 },
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "latestFundingRates",
                         "type": {
                             "array": [
                                 {
                                     "defined": "AnchorDecimal"
                                 },
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "latestFundingRatesPadding",
                         "type": {
                             "array": [
                                 {
                                     "defined": "AnchorDecimal"
                                 },
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "latestMidpoints",
                         "type": {
                             "array": [
                                 "u64",
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "latestMidpointsPadding",
                         "type": {
                             "array": [
                                 "u64",
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "oracles",
                         "type": {
                             "array": [
                                 "publicKey",
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "oraclesPadding",
                         "type": {
                             "array": [
                                 "publicKey",
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "oracleBackupFeeds",
                         "type": {
                             "array": [
                                 "publicKey",
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "oracleBackupFeedsPadding",
                         "type": {
                             "array": [
                                 "publicKey",
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "markets",
                         "type": {
                             "array": [
                                 "publicKey",
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "marketsPadding",
                         "type": {
                             "array": [
                                 "publicKey",
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "perpSyncQueues",
                         "type": {
                             "array": [
                                 "publicKey",
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "perpSyncQueuesPadding",
                         "type": {
                             "array": [
                                 "publicKey",
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "perpParameters",
                         "type": {
                             "array": [
                                 {
                                     "defined": "PerpParameters"
                                 },
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "perpParametersPadding",
                         "type": {
                             "array": [
                                 {
                                     "defined": "PerpParameters"
                                 },
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "marginParameters",
                         "type": {
                             "array": [
                                 {
                                     "defined": "MarginParameters"
                                 },
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "marginParametersPadding",
                         "type": {
                             "array": [
                                 {
                                     "defined": "MarginParameters"
                                 },
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "products",
                         "type": {
                             "array": [
                                 {
                                     "defined": "Product"
                                 },
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "productsPadding",
                         "type": {
                             "array": [
                                 {
                                     "defined": "Product"
                                 },
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "zetaGroupKeys",
                         "type": {
                             "array": [
                                 "publicKey",
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "zetaGroupKeysPadding",
                         "type": {
                             "array": [
                                 "publicKey",
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "totalInsuranceVaultDeposits",
                         "type": "u64"
                     },
@@ -275,24 +275,24 @@
                         "type": "i64"
                     },
                     {
                         "name": "haltForcePricing",
                         "type": {
                             "array": [
                                 "bool",
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "haltForcePricingPadding",
                         "type": {
                             "array": [
                                 "bool",
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "padding",
                         "type": {
                             "array": [
@@ -678,26 +678,26 @@
                     {
                         "name": "haltStates",
                         "type": {
                             "array": [
                                 {
                                     "defined": "HaltStateV2"
                                 },
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "haltStatesPadding",
                         "type": {
                             "array": [
                                 {
                                     "defined": "HaltStateV2"
                                 },
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "triggerAdmin",
                         "type": "publicKey"
                     },
@@ -1107,72 +1107,72 @@
                         }
                     },
                     {
                         "name": "openOrdersNonces",
                         "type": {
                             "array": [
                                 "u8",
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "openOrdersNoncesPadding",
                         "type": {
                             "array": [
                                 "u8",
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "rebalanceAmount",
                         "type": "i64"
                     },
                     {
                         "name": "lastFundingDeltas",
                         "type": {
                             "array": [
                                 {
                                     "defined": "AnchorDecimal"
                                 },
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "lastFundingDeltasPadding",
                         "type": {
                             "array": [
                                 {
                                     "defined": "AnchorDecimal"
                                 },
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "productLedgers",
                         "type": {
                             "array": [
                                 {
                                     "defined": "ProductLedger"
                                 },
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "productLedgersPadding",
                         "type": {
                             "array": [
                                 {
                                     "defined": "ProductLedger"
                                 },
-                                19
+                                18
                             ]
                         }
                     },
                     {
                         "name": "triggerOrderBits",
                         "type": "u128"
                     },
@@ -3000,15 +3000,15 @@
                 {
                     "isMut": true,
                     "isSigner": false,
                     "name": "crossMarginAccountManager"
                 },
                 {
                     "isMut": false,
-                    "isSigner": true,
+                    "isSigner": false,
                     "name": "authority"
                 },
                 {
                     "isMut": true,
                     "isSigner": true,
                     "name": "payer"
                 },
@@ -3036,15 +3036,15 @@
                 {
                     "isMut": true,
                     "isSigner": false,
                     "name": "crossMarginAccountManager"
                 },
                 {
                     "isMut": false,
-                    "isSigner": true,
+                    "isSigner": false,
                     "name": "authority"
                 },
                 {
                     "isMut": true,
                     "isSigner": true,
                     "name": "payer"
                 },
@@ -9284,15 +9284,15 @@
             "type": {
                 "fields": [
                     {
                         "name": "spotPrices",
                         "type": {
                             "array": [
                                 "u64",
-                                6
+                                7
                             ]
                         }
                     },
                     {
                         "name": "timestamp",
                         "type": "u64"
                     }
@@ -10085,14 +10085,17 @@
                     {
                         "name": "ARB"
                     },
                     {
                         "name": "BNB"
                     },
                     {
+                        "name": "PYTH"
+                    },
+                    {
                         "name": "UNDEFINED"
                     }
                 ]
             }
         },
         {
             "name": "MovementType",
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/market.py` & `zetamarkets_py-0.2.9/zetamarkets_py/market.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/orderbook.py` & `zetamarkets_py-0.2.9/zetamarkets_py/orderbook.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/pda.py` & `zetamarkets_py-0.2.9/zetamarkets_py/pda.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/risk.py` & `zetamarkets_py-0.2.9/zetamarkets_py/risk.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/__pycache__/market.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/__pycache__/market.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/__pycache__/market_state.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/__pycache__/market_state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/__pycache__/open_orders.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/__pycache__/open_orders.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/__pycache__/orderbook.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/__pycache__/orderbook.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/__pycache__/queue.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/__pycache__/queue.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/market_state.py` & `zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/market_state.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/open_orders.py` & `zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/open_orders.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/orderbook.py` & `zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/orderbook.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/serum_client/accounts/queue.py` & `zetamarkets_py-0.2.9/zetamarkets_py/serum_client/accounts/queue.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/serum_client/types/__pycache__/account_flags.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/serum_client/types/__pycache__/account_flags.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/serum_client/types/__pycache__/queue.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/serum_client/types/__pycache__/queue.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/serum_client/types/__pycache__/slab.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/serum_client/types/__pycache__/slab.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/serum_client/types/account_flags.py` & `zetamarkets_py-0.2.9/zetamarkets_py/serum_client/types/account_flags.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/serum_client/types/queue.py` & `zetamarkets_py-0.2.9/zetamarkets_py/serum_client/types/queue.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/serum_client/types/slab.py` & `zetamarkets_py-0.2.9/zetamarkets_py/serum_client/types/slab.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/solana_client/accounts/__pycache__/clock.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/solana_client/accounts/__pycache__/clock.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/solana_client/accounts/clock.py` & `zetamarkets_py-0.2.9/zetamarkets_py/solana_client/accounts/clock.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/types.py` & `zetamarkets_py-0.2.9/zetamarkets_py/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
     SOL = "SOL"
     BTC = "BTC"
     ETH = "ETH"
     APT = "APT"
     ARB = "ARB"
     BNB = "BNB"
+    PYTH = "PYTH"
 
     def to_index(self):
         """Converts the asset to its corresponding index."""
         members = list(self.__class__.__members__.values())
         return members.index(self)
 
     @classmethod
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/utils.py` & `zetamarkets_py-0.2.9/zetamarkets_py/utils.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/__init__.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/cross_margin_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/cross_margin_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/cross_margin_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/margin_account.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Aug 22 22:06:52 2023 UTC, .py size: 8516 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 7c31 e564 4421 0000  a.......|1.dD!..
+00000000: 610d 0d0a 0000 0000 1f64 e364 4e1f 0000  a........d.dN...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a04 6400 6403 6c05  ..d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6400 6407 6c0d  d.l.m.Z...d.d.l.
@@ -21,369 +21,336 @@
 00000140: 01da 1567 6574 5f6d 756c 7469 706c 655f  ...get_multiple_
 00000150: 6163 636f 756e 7473 2901 da0b 4173 796e  accounts)...Asyn
 00000160: 6343 6c69 656e 7429 01da 0a43 6f6d 6d69  cClient)...Commi
 00000170: 746d 656e 7429 01da 0650 7562 6b65 79e9  tment)...Pubkey.
 00000180: 0200 0000 2901 da05 7479 7065 7329 01da  ....)...types)..
 00000190: 0a50 524f 4752 414d 5f49 4463 0000 0000  .PROGRAM_IDc....
 000001a0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-000001b0: 4000 0000 73b6 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-000001c0: 0255 0065 0365 0464 013c 0065 0365 0464  .U.e.e.d.<.e.e.d
-000001d0: 023c 0065 0565 0464 033c 0065 0565 0464  .<.e.e.d.<.e.e.d
-000001e0: 043c 0065 0565 0464 053c 0065 0665 0464  .<.e.e.d.<.e.e.d
-000001f0: 063c 0065 076a 086a 0965 0464 073c 0065  .<.e.j.j.e.d.<.e
-00000200: 0a65 0519 0065 0464 083c 0065 0a65 0519  .e...e.d.<.e.e..
-00000210: 0065 0464 093c 0065 0565 0464 0a3c 0065  .e.d.<.e.e.d.<.e
-00000220: 0a65 076a 0b6a 0c19 0065 0464 0b3c 0065  .e.j.j...e.d.<.e
-00000230: 0a65 076a 0b6a 0c19 0065 0464 0c3c 0065  .e.j.j...e.d.<.e
-00000240: 0a65 076a 0d6a 0e19 0065 0464 0d3c 0065  .e.j.j...e.d.<.e
-00000250: 0a65 076a 0d6a 0e19 0065 0464 0e3c 0065  .e.j.j...e.d.<.e
-00000260: 0a65 0519 0065 0464 0f3c 0064 1053 0029  .e...e.d.<.d.S.)
-00000270: 11da 1643 726f 7373 4d61 7267 696e 4163  ...CrossMarginAc
-00000280: 636f 756e 744a 534f 4eda 0961 7574 686f  countJSON..autho
-00000290: 7269 7479 da10 6465 6c65 6761 7465 645f  rity..delegated_
-000002a0: 7075 626b 6579 da07 6261 6c61 6e63 65da  pubkey..balance.
-000002b0: 1073 7562 6163 636f 756e 745f 696e 6465  .subaccount_inde
-000002c0: 78da 056e 6f6e 6365 da11 666f 7263 655f  x..nonce..force_
-000002d0: 6361 6e63 656c 5f66 6c61 67da 0c61 6363  cancel_flag..acc
-000002e0: 6f75 6e74 5f74 7970 65da 126f 7065 6e5f  ount_type..open_
-000002f0: 6f72 6465 7273 5f6e 6f6e 6365 73da 1a6f  orders_nonces..o
-00000300: 7065 6e5f 6f72 6465 7273 5f6e 6f6e 6365  pen_orders_nonce
-00000310: 735f 7061 6464 696e 67da 1072 6562 616c  s_padding..rebal
-00000320: 616e 6365 5f61 6d6f 756e 74da 136c 6173  ance_amount..las
-00000330: 745f 6675 6e64 696e 675f 6465 6c74 6173  t_funding_deltas
-00000340: da1b 6c61 7374 5f66 756e 6469 6e67 5f64  ..last_funding_d
-00000350: 656c 7461 735f 7061 6464 696e 67da 0f70  eltas_padding..p
-00000360: 726f 6475 6374 5f6c 6564 6765 7273 da17  roduct_ledgers..
-00000370: 7072 6f64 7563 745f 6c65 6467 6572 735f  product_ledgers_
-00000380: 7061 6464 696e 67da 0770 6164 6469 6e67  padding..padding
-00000390: 4e29 0fda 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-000003a0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-000003b0: 6c6e 616d 655f 5fda 0373 7472 da0f 5f5f  lname__..str..__
-000003c0: 616e 6e6f 7461 7469 6f6e 735f 5fda 0369  annotations__..i
-000003d0: 6e74 da04 626f 6f6c 720b 0000 00da 136d  nt..boolr......m
-000003e0: 6172 6769 6e5f 6163 636f 756e 745f 7479  argin_account_ty
-000003f0: 7065 5a15 4d61 7267 696e 4163 636f 756e  peZ.MarginAccoun
-00000400: 7454 7970 654a 534f 4eda 046c 6973 74da  tTypeJSON..list.
-00000410: 0e61 6e63 686f 725f 6465 6369 6d61 6c5a  .anchor_decimalZ
-00000420: 1141 6e63 686f 7244 6563 696d 616c 4a53  .AnchorDecimalJS
-00000430: 4f4e da0e 7072 6f64 7563 745f 6c65 6467  ON..product_ledg
-00000440: 6572 5a11 5072 6f64 7563 744c 6564 6765  erZ.ProductLedge
-00000450: 724a 534f 4ea9 0072 2800 0000 7228 0000  rJSON..r(...r(..
-00000460: 00fa 5a2f 5573 6572 732f 7466 7269 7a7a  ..Z/Users/tfrizz
-00000470: 612f 446f 6375 6d65 6e74 732f 7a65 7461  a/Documents/zeta
-00000480: 2f7a 6574 612d 7079 2f7a 6574 615f 7079  /zeta-py/zeta_py
-00000490: 2f7a 6574 615f 636c 6965 6e74 2f61 6363  /zeta_client/acc
-000004a0: 6f75 6e74 732f 6372 6f73 735f 6d61 7267  ounts/cross_marg
-000004b0: 696e 5f61 6363 6f75 6e74 2e70 7972 0d00  in_account.pyr..
-000004c0: 0000 1100 0000 731e 0000 000a 0108 0108  ......s.........
-000004d0: 0108 0108 0108 0108 010c 010c 010c 0108  ................
-000004e0: 0110 0110 0110 0110 0172 0d00 0000 6300  .........r....c.
-000004f0: 0000 0000 0000 0000 0000 0000 0000 0013  ................
-00000500: 0000 0040 0000 0073 0e02 0000 6500 5a01  ...@...s....e.Z.
+000001b0: 4000 0000 73ba 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+000001c0: 0255 0065 0365 0464 013c 0065 0565 0464  .U.e.e.d.<.e.e.d
+000001d0: 023c 0065 0565 0464 033c 0065 0665 0464  .<.e.e.d.<.e.e.d
+000001e0: 043c 0065 0765 0519 0065 0464 053c 0065  .<.e.e...e.d.<.e
+000001f0: 0765 0519 0065 0464 063c 0065 0565 0464  .e...e.d.<.e.e.d
+00000200: 073c 0065 0765 086a 096a 0a19 0065 0464  .<.e.e.j.j...e.d
+00000210: 083c 0065 0765 086a 096a 0a19 0065 0464  .<.e.e.j.j...e.d
+00000220: 093c 0065 086a 096a 0a65 0464 0a3c 0065  .<.e.j.j.e.d.<.e
+00000230: 0565 0464 0b3c 0065 086a 0b6a 0c65 0464  .e.d.<.e.j.j.e.d
+00000240: 0c3c 0065 086a 0d6a 0e65 0464 0d3c 0065  .<.e.j.j.e.d.<.e
+00000250: 086a 0f6a 1065 0464 0e3c 0065 0365 0464  .j.j.e.d.<.e.e.d
+00000260: 0f3c 0065 0765 0519 0065 0464 103c 0064  .<.e.e...e.d.<.d
+00000270: 1153 0029 12da 114d 6172 6769 6e41 6363  .S.)...MarginAcc
+00000280: 6f75 6e74 4a53 4f4e da09 6175 7468 6f72  ountJSON..author
+00000290: 6974 79da 056e 6f6e 6365 da07 6261 6c61  ity..nonce..bala
+000002a0: 6e63 65da 1166 6f72 6365 5f63 616e 6365  nce..force_cance
+000002b0: 6c5f 666c 6167 da11 6f70 656e 5f6f 7264  l_flag..open_ord
+000002c0: 6572 735f 6e6f 6e63 65da 0d73 6572 6965  ers_nonce..serie
+000002d0: 735f 6578 7069 7279 da15 7365 7269 6573  s_expiry..series
+000002e0: 5f65 7870 6972 795f 7061 6464 696e 67da  _expiry_padding.
+000002f0: 0f70 726f 6475 6374 5f6c 6564 6765 7273  .product_ledgers
+00000300: da17 7072 6f64 7563 745f 6c65 6467 6572  ..product_ledger
+00000310: 735f 7061 6464 696e 67da 1370 6572 705f  s_padding..perp_
+00000320: 7072 6f64 7563 745f 6c65 6467 6572 da10  product_ledger..
+00000330: 7265 6261 6c61 6e63 655f 616d 6f75 6e74  rebalance_amount
+00000340: da05 6173 7365 74da 0c61 6363 6f75 6e74  ..asset..account
+00000350: 5f74 7970 65da 126c 6173 745f 6675 6e64  _type..last_fund
+00000360: 696e 675f 6465 6c74 61da 1064 656c 6567  ing_delta..deleg
+00000370: 6174 6564 5f70 7562 6b65 79da 0770 6164  ated_pubkey..pad
+00000380: 6469 6e67 4e29 11da 085f 5f6e 616d 655f  dingN)...__name_
+00000390: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+000003a0: 5f71 7561 6c6e 616d 655f 5fda 0373 7472  _qualname__..str
+000003b0: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
+000003c0: 5fda 0369 6e74 da04 626f 6f6c da04 6c69  _..int..bool..li
+000003d0: 7374 720b 0000 00da 0e70 726f 6475 6374  str......product
+000003e0: 5f6c 6564 6765 72da 1150 726f 6475 6374  _ledger..Product
+000003f0: 4c65 6467 6572 4a53 4f4e 7219 0000 00da  LedgerJSONr.....
+00000400: 0941 7373 6574 4a53 4f4e da13 6d61 7267  .AssetJSON..marg
+00000410: 696e 5f61 6363 6f75 6e74 5f74 7970 65da  in_account_type.
+00000420: 154d 6172 6769 6e41 6363 6f75 6e74 5479  .MarginAccountTy
+00000430: 7065 4a53 4f4e da0e 616e 6368 6f72 5f64  peJSON..anchor_d
+00000440: 6563 696d 616c da11 416e 6368 6f72 4465  ecimal..AnchorDe
+00000450: 6369 6d61 6c4a 534f 4ea9 0072 2d00 0000  cimalJSON..r-...
+00000460: 722d 0000 00fa 542f 5573 6572 732f 7466  r-....T/Users/tf
+00000470: 7269 7a7a 612f 446f 6375 6d65 6e74 732f  rizza/Documents/
+00000480: 7a65 7461 2f7a 6574 612d 7079 2f7a 6574  zeta/zeta-py/zet
+00000490: 615f 7079 2f7a 6574 615f 636c 6965 6e74  a_py/zeta_client
+000004a0: 2f61 6363 6f75 6e74 732f 6d61 7267 696e  /accounts/margin
+000004b0: 5f61 6363 6f75 6e74 2e70 7972 0d00 0000  _account.pyr....
+000004c0: 1100 0000 7320 0000 000a 0108 0108 0108  ....s ..........
+000004d0: 0108 010c 010c 0108 0110 0110 010c 0108  ................
+000004e0: 010c 010c 010c 0108 0172 0d00 0000 6300  .........r....c.
+000004f0: 0000 0000 0000 0000 0000 0000 0000 0014  ................
+00000500: 0000 0040 0000 0073 1602 0000 6500 5a01  ...@...s....e.Z.
 00000510: 6400 5a02 5500 6401 5a03 6504 6a05 6506  d.Z.U.d.Z.e.j.e.
 00000520: 6402 3c00 6507 a008 6403 6509 1b00 6404  d.<.e...d.e...d.
-00000530: 6509 1b00 6405 6507 6a0a 1b00 6406 6507  e...d.e.j...d.e.
-00000540: 6a0b 1b00 6407 6507 6a0b 1b00 6408 6507  j...d.e.j...d.e.
-00000550: 6a0c 1b00 6409 650d 6a0e 6a0f 1b00 640a  j...d.e.j.j...d.
-00000560: 6507 6a0b 640b 1900 1b00 640c 6507 6a0b  e.j.d.....d.e.j.
-00000570: 640d 1900 1b00 640e 6507 6a10 1b00 640f  d.....d.e.j...d.
-00000580: 650d 6a11 6a12 6a0f 640b 1900 1b00 6410  e.j.j.j.d.....d.
-00000590: 650d 6a11 6a12 6a0f 640d 1900 1b00 6411  e.j.j.j.d.....d.
-000005a0: 650d 6a13 6a14 6a0f 640b 1900 1b00 6412  e.j.j.j.d.....d.
-000005b0: 650d 6a13 6a14 6a0f 640d 1900 1b00 6413  e.j.j.j.d.....d.
-000005c0: 6507 6a0b 6414 1900 1b00 a10f 5a0f 6504  e.j.d.......Z.e.
-000005d0: 6a05 6506 6415 3c00 6515 6506 6403 3c00  j.e.d.<.e.e.d.<.
-000005e0: 6515 6506 6404 3c00 6516 6506 6405 3c00  e.e.d.<.e.e.d.<.
-000005f0: 6516 6506 6406 3c00 6516 6506 6407 3c00  e.e.d.<.e.e.d.<.
-00000600: 6517 6506 6408 3c00 650d 6a0e 6a18 6506  e.e.d.<.e.j.j.e.
-00000610: 6409 3c00 6519 6516 1900 6506 640a 3c00  d.<.e.e...e.d.<.
-00000620: 6519 6516 1900 6506 640c 3c00 6516 6506  e.e...e.d.<.e.e.
-00000630: 640e 3c00 6519 650d 6a11 6a12 1900 6506  d.<.e.e.j.j...e.
-00000640: 640f 3c00 6519 650d 6a11 6a12 1900 6506  d.<.e.e.j.j...e.
-00000650: 6410 3c00 6519 650d 6a13 6a14 1900 6506  d.<.e.e.j.j...e.
-00000660: 6411 3c00 6519 650d 6a13 6a14 1900 6506  d.<.e.e.j.j...e.
-00000670: 6412 3c00 6519 6516 1900 6506 6413 3c00  d.<.e.e...e.d.<.
-00000680: 651a 6416 651b 6602 651c 6515 6504 6a1d  e.d.e.f.e.e.e.j.
-00000690: 651e 1900 6515 6504 6a1d 6400 1900 6417  e...e.e.j.d...d.
-000006a0: 9c05 6418 6419 8405 8301 5a1f 651a 6416  ..d.d.....Z.e.d.
-000006b0: 651b 6602 651c 6519 6515 1900 6504 6a1d  e.f.e.e.e...e.j.
-000006c0: 651e 1900 6515 6519 6504 6a1d 6400 1900  e...e.e.e.j.d...
-000006d0: 1900 641a 9c05 641b 641c 8405 8301 5a20  ..d...d.d.....Z 
-000006e0: 651a 6521 6400 641d 9c02 641e 641f 8404  e.e!d.d...d.d...
-000006f0: 8301 5a22 6523 6420 9c01 6421 6422 8404  ..Z"e#d ..d!d"..
-00000700: 5a24 651a 6523 6400 6423 9c02 6424 6425  Z$e.e#d.d#..d$d%
-00000710: 8404 8301 5a25 6416 5300 2926 da12 4372  ....Z%d.S.)&..Cr
-00000720: 6f73 734d 6172 6769 6e41 6363 6f75 6e74  ossMarginAccount
-00000730: 7308 0000 00f2 5e8e 8323 f493 1cda 0d64  s.....^..#.....d
-00000740: 6973 6372 696d 696e 6174 6f72 720e 0000  iscriminatorr...
-00000750: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
-00000760: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-00000770: 1500 0000 e905 0000 0072 1600 0000 e914  .........r......
-00000780: 0000 0072 1700 0000 7218 0000 0072 1900  ...r....r....r..
-00000790: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-000007a0: 0069 d007 0000 da06 6c61 796f 7574 4e29  .i......layoutN)
-000007b0: 05da 0463 6f6e 6eda 0761 6464 7265 7373  ...conn..address
-000007c0: da0a 636f 6d6d 6974 6d65 6e74 da0a 7072  ..commitment..pr
-000007d0: 6f67 7261 6d5f 6964 da06 7265 7475 726e  ogram_id..return
-000007e0: 6305 0000 0000 0000 0000 0000 0008 0000  c...............
-000007f0: 0004 0000 00c3 0000 0073 4800 0000 7c01  .........sH...|.
-00000800: 6a00 7c02 7c03 6401 8d02 4900 6400 4800  j.|.|.d...I.d.H.
-00000810: 7d05 7c05 6a01 7d06 7c06 6400 7500 7226  }.|.j.}.|.d.u.r&
-00000820: 6400 5300 7c06 6a02 7c04 6b03 7238 7403  d.S.|.j.|.k.r8t.
-00000830: 6402 8301 8201 7c06 6a04 7d07 7c00 a005  d.....|.j.}.|...
-00000840: 7c07 a101 5300 a903 4e29 0172 3100 0000  |...S...N).r1...
-00000850: 7a27 4163 636f 756e 7420 646f 6573 206e  z'Account does n
-00000860: 6f74 2062 656c 6f6e 6720 746f 2074 6869  ot belong to thi
-00000870: 7320 7072 6f67 7261 6d29 065a 1067 6574  s program).Z.get
-00000880: 5f61 6363 6f75 6e74 5f69 6e66 6fda 0576  _account_info..v
-00000890: 616c 7565 da05 6f77 6e65 72da 0a56 616c  alue..owner..Val
-000008a0: 7565 4572 726f 72da 0464 6174 61da 0664  ueError..data..d
-000008b0: 6563 6f64 6529 08da 0363 6c73 722f 0000  ecode)...clsr/..
-000008c0: 0072 3000 0000 7231 0000 0072 3200 0000  .r0...r1...r2...
-000008d0: da04 7265 7370 da04 696e 666f da0a 6279  ..resp..info..by
-000008e0: 7465 735f 6461 7461 7228 0000 0072 2800  tes_datar(...r(.
-000008f0: 0000 7229 0000 00da 0566 6574 6368 4700  ..r).....fetchG.
-00000900: 0000 7310 0000 0000 0814 0106 0108 0104  ..s.............
-00000910: 010a 0108 0106 017a 1843 726f 7373 4d61  .......z.CrossMa
-00000920: 7267 696e 4163 636f 756e 742e 6665 7463  rginAccount.fetc
-00000930: 6829 0572 2f00 0000 da09 6164 6472 6573  h).r/.....addres
-00000940: 7365 7372 3100 0000 7232 0000 0072 3300  sesr1...r2...r3.
-00000950: 0000 6305 0000 0000 0000 0000 0000 0008  ..c.............
-00000960: 0000 0006 0000 00c3 0000 0073 6200 0000  ...........sb...
-00000970: 7400 7c01 7c02 7c03 6401 8d03 4900 6400  t.|.|.|.d...I.d.
-00000980: 4800 7d05 6700 7d06 7c05 4400 5d40 7d07  H.}.g.}.|.D.]@}.
-00000990: 7c07 6400 7500 7234 7c06 a001 6400 a101  |.d.u.r4|...d...
-000009a0: 0100 711c 7c07 6a02 6a03 7c04 6b03 7248  ..q.|.j.j.|.k.rH
-000009b0: 7404 6402 8301 8201 7c06 a001 7c00 a005  t.d.....|...|...
-000009c0: 7c07 6a02 6a06 a101 a101 0100 711c 7c06  |.j.j.......q.|.
-000009d0: 5300 7234 0000 0029 0772 0600 0000 da06  S.r4...).r......
-000009e0: 6170 7065 6e64 da07 6163 636f 756e 7472  append..accountr
-000009f0: 3600 0000 7237 0000 0072 3900 0000 7238  6...r7...r9...r8
-00000a00: 0000 0029 0872 3a00 0000 722f 0000 0072  ...).r:...r/...r
-00000a10: 3f00 0000 7231 0000 0072 3200 0000 da05  ?...r1...r2.....
-00000a20: 696e 666f 73da 0372 6573 723c 0000 0072  infos..resr<...r
-00000a30: 2800 0000 7228 0000 0072 2900 0000 da0e  (...r(...r).....
-00000a40: 6665 7463 685f 6d75 6c74 6970 6c65 5800  fetch_multipleX.
-00000a50: 0000 7314 0000 0000 0814 0104 0108 0108  ..s.............
-00000a60: 010a 0102 010c 0108 0116 017a 2143 726f  ...........z!Cro
-00000a70: 7373 4d61 7267 696e 4163 636f 756e 742e  ssMarginAccount.
-00000a80: 6665 7463 685f 6d75 6c74 6970 6c65 2902  fetch_multiple).
-00000a90: 7238 0000 0072 3300 0000 6302 0000 0000  r8...r3...c.....
-00000aa0: 0000 0000 0000 0003 0000 0012 0000 0043  ...............C
-00000ab0: 0000 0073 b200 0000 7c01 6400 7400 8502  ...s....|.d.t...
-00000ac0: 1900 7c00 6a01 6b03 721a 7402 6401 8301  ..|.j.k.r.t.d...
-00000ad0: 8201 7403 6a04 a005 7c01 7400 6400 8502  ..t.j...|.t.d...
-00000ae0: 1900 a101 7d02 7c00 7c02 6a06 7c02 6a07  ....}.|.|.j.|.j.
-00000af0: 7c02 6a08 7c02 6a09 7c02 6a0a 7c02 6a0b  |.j.|.j.|.j.|.j.
-00000b00: 740c 6a0d a00e 7c02 6a0f a101 7c02 6a10  t.j...|.j...|.j.
-00000b10: 7c02 6a11 7c02 6a12 7413 7414 6402 6403  |.j.|.j.t.t.d.d.
-00000b20: 8400 7c02 6a15 8302 8301 7413 7414 6404  ..|.j.....t.t.d.
-00000b30: 6403 8400 7c02 6a16 8302 8301 7413 7414  d...|.j.....t.t.
-00000b40: 6405 6403 8400 7c02 6a17 8302 8301 7413  d.d...|.j.....t.
-00000b50: 7414 6406 6403 8400 7c02 6a18 8302 8301  t.d.d...|.j.....
-00000b60: 7c02 6a19 6407 8d0f 5300 2908 4e7a 2d54  |.j.d...S.).Nz-T
-00000b70: 6865 2064 6973 6372 696d 696e 6174 6f72  he discriminator
-00000b80: 2066 6f72 2074 6869 7320 6163 636f 756e   for this accoun
-00000b90: 7420 6973 2069 6e76 616c 6964 6301 0000  t is invalidc...
-00000ba0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00000bb0: 0053 0000 0073 0e00 0000 7400 6a01 6a02  .S...s....t.j.j.
-00000bc0: a003 7c00 a101 5300 a901 4ea9 0472 0b00  ..|...S...N..r..
-00000bd0: 0000 7226 0000 00da 0d41 6e63 686f 7244  ..r&.....AnchorD
-00000be0: 6563 696d 616c da0c 6672 6f6d 5f64 6563  ecimal..from_dec
-00000bf0: 6f64 6564 a901 da04 6974 656d 7228 0000  oded....itemr(..
-00000c00: 0072 2800 0000 7229 0000 00da 083c 6c61  .r(...r).....<la
-00000c10: 6d62 6461 3e7d 0000 00f3 0000 0000 7a2b  mbda>}........z+
-00000c20: 4372 6f73 734d 6172 6769 6e41 6363 6f75  CrossMarginAccou
-00000c30: 6e74 2e64 6563 6f64 652e 3c6c 6f63 616c  nt.decode.<local
-00000c40: 733e 2e3c 6c61 6d62 6461 3e63 0100 0000  s>.<lambda>c....
-00000c50: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00000c60: 5300 0000 730e 0000 0074 006a 016a 02a0  S...s....t.j.j..
-00000c70: 037c 00a1 0153 0072 4500 0000 7246 0000  .|...S.rE...rF..
-00000c80: 0072 4900 0000 7228 0000 0072 2800 0000  .rI...r(...r(...
-00000c90: 7229 0000 0072 4b00 0000 8300 0000 724c  r)...rK.......rL
-00000ca0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000cb0: 0100 0000 0300 0000 5300 0000 730e 0000  ........S...s...
-00000cc0: 0074 006a 016a 02a0 037c 00a1 0153 0072  .t.j.j...|...S.r
-00000cd0: 4500 0000 a904 720b 0000 0072 2700 0000  E.....r....r'...
-00000ce0: da0d 5072 6f64 7563 744c 6564 6765 7272  ..ProductLedgerr
-00000cf0: 4800 0000 7249 0000 0072 2800 0000 7228  H...rI...r(...r(
-00000d00: 0000 0072 2900 0000 724b 0000 0089 0000  ...r)...rK......
-00000d10: 0072 4c00 0000 6301 0000 0000 0000 0000  .rL...c.........
-00000d20: 0000 0001 0000 0003 0000 0053 0000 0073  ...........S...s
-00000d30: 0e00 0000 7400 6a01 6a02 a003 7c00 a101  ....t.j.j...|...
-00000d40: 5300 7245 0000 0072 4d00 0000 7249 0000  S.rE...rM...rI..
-00000d50: 0072 2800 0000 7228 0000 0072 2900 0000  .r(...r(...r)...
-00000d60: 724b 0000 008f 0000 0072 4c00 0000 a90f  rK.......rL.....
-00000d70: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00000d80: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
-00000d90: 0000 0072 1500 0000 7216 0000 0072 1700  ...r....r....r..
-00000da0: 0000 7218 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00000db0: 0072 1b00 0000 721c 0000 0029 1a72 0400  .r....r....).r..
-00000dc0: 0000 722b 0000 0072 0500 0000 722a 0000  ..r+...r....r*..
-00000dd0: 0072 2e00 0000 da05 7061 7273 6572 0e00  .r......parser..
-00000de0: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00000df0: 0072 1200 0000 7213 0000 0072 0b00 0000  .r....r....r....
-00000e00: 7224 0000 0072 4800 0000 7214 0000 0072  r$...rH...r....r
-00000e10: 1500 0000 7216 0000 0072 1700 0000 7225  ....r....r....r%
-00000e20: 0000 00da 036d 6170 7218 0000 0072 1900  .....mapr....r..
-00000e30: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-00000e40: 0029 0372 3a00 0000 7238 0000 00da 0364  .).r:...r8.....d
-00000e50: 6563 7228 0000 0072 2800 0000 7229 0000  ecr(...r(...r)..
-00000e60: 0072 3900 0000 6b00 0000 7350 0000 0000  .r9...k...sP....
-00000e70: 0212 0108 0114 0102 0104 0104 0104 0104  ................
-00000e80: 0104 0104 010c 0104 0104 0104 0102 0102  ................
-00000e90: 0106 0104 fe02 ff02 0602 0102 0106 0104  ................
-00000ea0: fe02 ff02 0602 0102 0106 0104 fe02 ff02  ................
-00000eb0: 0602 0102 0106 0104 fe02 ff02 0604 dd7a  ...............z
-00000ec0: 1943 726f 7373 4d61 7267 696e 4163 636f  .CrossMarginAcco
-00000ed0: 756e 742e 6465 636f 6465 2901 7233 0000  unt.decode).r3..
-00000ee0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00000ef0: 0000 1100 0000 4300 0000 7386 0000 0074  ......C...s....t
-00000f00: 007c 006a 0183 0174 007c 006a 0283 017c  .|.j...t.|.j...|
-00000f10: 006a 037c 006a 047c 006a 057c 006a 067c  .j.|.j.|.j.|.j.|
-00000f20: 006a 07a0 08a1 007c 006a 097c 006a 0a7c  .j.....|.j.|.j.|
-00000f30: 006a 0b74 0c74 0d64 0164 0284 007c 006a  .j.t.t.d.d...|.j
-00000f40: 0e83 0283 0174 0c74 0d64 0364 0284 007c  .....t.t.d.d...|
-00000f50: 006a 0f83 0283 0174 0c74 0d64 0464 0284  .j.....t.t.d.d..
-00000f60: 007c 006a 1083 0283 0174 0c74 0d64 0564  .|.j.....t.t.d.d
-00000f70: 0284 007c 006a 1183 0283 017c 006a 1264  ...|.j.....|.j.d
-00000f80: 069c 0f53 0029 074e 6301 0000 0000 0000  ...S.).Nc.......
-00000f90: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
-00000fa0: 0073 0800 0000 7c00 a000 a100 5300 7245  .s....|.....S.rE
-00000fb0: 0000 00a9 01da 0774 6f5f 6a73 6f6e 7249  .......to_jsonrI
-00000fc0: 0000 0072 2800 0000 7228 0000 0072 2900  ...r(...r(...r).
-00000fd0: 0000 724b 0000 00a2 0000 0072 4c00 0000  ..rK.......rL...
-00000fe0: 7a2c 4372 6f73 734d 6172 6769 6e41 6363  z,CrossMarginAcc
-00000ff0: 6f75 6e74 2e74 6f5f 6a73 6f6e 2e3c 6c6f  ount.to_json.<lo
-00001000: 6361 6c73 3e2e 3c6c 616d 6264 613e 6301  cals>.<lambda>c.
-00001010: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00001020: 0000 0053 0000 0073 0800 0000 7c00 a000  ...S...s....|...
-00001030: a100 5300 7245 0000 0072 5300 0000 7249  ..S.rE...rS...rI
-00001040: 0000 0072 2800 0000 7228 0000 0072 2900  ...r(...r(...r).
-00001050: 0000 724b 0000 00a3 0000 0072 4c00 0000  ..rK.......rL...
-00001060: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001070: 0002 0000 0053 0000 0073 0800 0000 7c00  .....S...s....|.
-00001080: a000 a100 5300 7245 0000 0072 5300 0000  ....S.rE...rS...
-00001090: 7249 0000 0072 2800 0000 7228 0000 0072  rI...r(...r(...r
-000010a0: 2900 0000 724b 0000 00a4 0000 0072 4c00  )...rK.......rL.
-000010b0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-000010c0: 0000 0002 0000 0053 0000 0073 0800 0000  .......S...s....
-000010d0: 7c00 a000 a100 5300 7245 0000 0072 5300  |.....S.rE...rS.
-000010e0: 0000 7249 0000 0072 2800 0000 7228 0000  ..rI...r(...r(..
-000010f0: 0072 2900 0000 724b 0000 00a5 0000 0072  .r)...rK.......r
-00001100: 4c00 0000 724f 0000 0029 1372 2000 0000  L...rO...).r ...
-00001110: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00001120: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
-00001130: 0000 0072 5400 0000 7215 0000 0072 1600  ...rT...r....r..
-00001140: 0000 7217 0000 0072 2500 0000 7251 0000  ..r....r%...rQ..
-00001150: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00001160: 721b 0000 0072 1c00 0000 2901 da04 7365  r....r....)...se
-00001170: 6c66 7228 0000 0072 2800 0000 7229 0000  lfr(...r(...r)..
-00001180: 0072 5400 0000 9600 0000 7320 0000 0000  .rT.......s ....
-00001190: 0208 0108 0104 0104 0104 0104 0108 0104  ................
-000011a0: 0104 0104 0112 0112 0112 0112 0104 f17a  ...............z
-000011b0: 1a43 726f 7373 4d61 7267 696e 4163 636f  .CrossMarginAcco
-000011c0: 756e 742e 746f 5f6a 736f 6e29 02da 036f  unt.to_json)...o
-000011d0: 626a 7233 0000 0063 0200 0000 0000 0000  bjr3...c........
-000011e0: 0000 0000 0200 0000 1300 0000 4300 0000  ............C...
-000011f0: 73ae 0000 007c 0074 00a0 017c 0164 0119  s....|.t...|.d..
-00001200: 00a1 0174 00a0 017c 0164 0219 00a1 017c  ...t...|.d.....|
-00001210: 0164 0319 007c 0164 0419 007c 0164 0519  .d...|.d...|.d..
-00001220: 007c 0164 0619 0074 026a 03a0 047c 0164  .|.d...t.j...|.d
-00001230: 0719 00a1 017c 0164 0819 007c 0164 0919  .....|.d...|.d..
-00001240: 007c 0164 0a19 0074 0574 0664 0b64 0c84  .|.d...t.t.d.d..
-00001250: 007c 0164 0d19 0083 0283 0174 0574 0664  .|.d.......t.t.d
-00001260: 0e64 0c84 007c 0164 0f19 0083 0283 0174  .d...|.d.......t
-00001270: 0574 0664 1064 0c84 007c 0164 1119 0083  .t.d.d...|.d....
-00001280: 0283 0174 0574 0664 1264 0c84 007c 0164  ...t.t.d.d...|.d
-00001290: 1319 0083 0283 017c 0164 1419 0064 158d  .......|.d...d..
-000012a0: 0f53 0029 164e 720e 0000 0072 0f00 0000  .S.).Nr....r....
-000012b0: 7210 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-000012c0: 1300 0000 7214 0000 0072 1500 0000 7216  ....r....r....r.
-000012d0: 0000 0072 1700 0000 6301 0000 0000 0000  ...r....c.......
-000012e0: 0000 0000 0001 0000 0003 0000 0053 0000  .............S..
-000012f0: 0073 0e00 0000 7400 6a01 6a02 a003 7c00  .s....t.j.j...|.
-00001300: a101 5300 7245 0000 00a9 0472 0b00 0000  ..S.rE.....r....
-00001310: 7226 0000 0072 4700 0000 da09 6672 6f6d  r&...rG.....from
-00001320: 5f6a 736f 6e72 4900 0000 7228 0000 0072  _jsonrI...r(...r
-00001330: 2800 0000 7229 0000 0072 4b00 0000 b800  (...r)...rK.....
-00001340: 0000 724c 0000 007a 2e43 726f 7373 4d61  ..rL...z.CrossMa
-00001350: 7267 696e 4163 636f 756e 742e 6672 6f6d  rginAccount.from
-00001360: 5f6a 736f 6e2e 3c6c 6f63 616c 733e 2e3c  _json.<locals>.<
-00001370: 6c61 6d62 6461 3e72 1800 0000 6301 0000  lambda>r....c...
-00001380: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00001390: 0053 0000 0073 0e00 0000 7400 6a01 6a02  .S...s....t.j.j.
-000013a0: a003 7c00 a101 5300 7245 0000 0072 5700  ..|...S.rE...rW.
-000013b0: 0000 7249 0000 0072 2800 0000 7228 0000  ..rI...r(...r(..
-000013c0: 0072 2900 0000 724b 0000 00be 0000 0072  .r)...rK.......r
-000013d0: 4c00 0000 7219 0000 0063 0100 0000 0000  L...r....c......
-000013e0: 0000 0000 0000 0100 0000 0300 0000 5300  ..............S.
-000013f0: 0000 730e 0000 0074 006a 016a 02a0 037c  ..s....t.j.j...|
-00001400: 00a1 0153 0072 4500 0000 a904 720b 0000  ...S.rE.....r...
-00001410: 0072 2700 0000 724e 0000 0072 5800 0000  .r'...rN...rX...
-00001420: 7249 0000 0072 2800 0000 7228 0000 0072  rI...r(...r(...r
-00001430: 2900 0000 724b 0000 00c4 0000 0072 4c00  )...rK.......rL.
-00001440: 0000 721a 0000 0063 0100 0000 0000 0000  ..r....c........
-00001450: 0000 0000 0100 0000 0300 0000 5300 0000  ............S...
-00001460: 730e 0000 0074 006a 016a 02a0 037c 00a1  s....t.j.j...|..
-00001470: 0153 0072 4500 0000 7259 0000 0072 4900  .S.rE...rY...rI.
-00001480: 0000 7228 0000 0072 2800 0000 7229 0000  ..r(...r(...r)..
-00001490: 0072 4b00 0000 ca00 0000 724c 0000 0072  .rK.......rL...r
-000014a0: 1b00 0000 721c 0000 0072 4f00 0000 2907  ....r....rO...).
-000014b0: 7209 0000 00da 0b66 726f 6d5f 7374 7269  r......from_stri
-000014c0: 6e67 720b 0000 0072 2400 0000 7258 0000  ngr....r$...rX..
-000014d0: 0072 2500 0000 7251 0000 0029 0272 3a00  .r%...rQ...).r:.
-000014e0: 0000 7256 0000 0072 2800 0000 7228 0000  ..rV...r(...r(..
-000014f0: 0072 2900 0000 7258 0000 00a9 0000 0073  .r)...rX.......s
-00001500: 4a00 0000 0002 0201 0c01 0c01 0601 0601  J...............
-00001510: 0601 0601 0e01 0601 0601 0601 0201 0201  ................
-00001520: 0601 06fe 02ff 0206 0201 0201 0601 06fe  ................
-00001530: 02ff 0206 0201 0201 0601 06fe 02ff 0206  ................
-00001540: 0201 0201 0601 06fe 02ff 0206 06dd 7a1c  ..............z.
-00001550: 4372 6f73 734d 6172 6769 6e41 6363 6f75  CrossMarginAccou
-00001560: 6e74 2e66 726f 6d5f 6a73 6f6e 2926 721d  nt.from_json)&r.
-00001570: 0000 0072 1e00 0000 721f 0000 0072 2b00  ...r....r....r+.
-00001580: 0000 da06 7479 7069 6e67 da08 436c 6173  ....typing..Clas
-00001590: 7356 6172 7221 0000 00da 0562 6f72 7368  sVarr!.....borsh
-000015a0: 5a07 4353 7472 7563 7472 0300 0000 5a03  Z.CStructr....Z.
-000015b0: 5536 345a 0255 38da 0442 6f6f 6c72 0b00  U64Z.U8..Boolr..
-000015c0: 0000 7224 0000 0072 2e00 0000 5a03 4936  ..r$...r....Z.I6
-000015d0: 3472 2600 0000 7247 0000 0072 2700 0000  4r&...rG...r'...
-000015e0: 724e 0000 0072 0900 0000 7222 0000 0072  rN...r....r"...r
-000015f0: 2300 0000 5a15 4d61 7267 696e 4163 636f  #...Z.MarginAcco
-00001600: 756e 7454 7970 654b 696e 6472 2500 0000  untTypeKindr%...
-00001610: da0b 636c 6173 736d 6574 686f 6472 0c00  ..classmethodr..
-00001620: 0000 7207 0000 00da 084f 7074 696f 6e61  ..r......Optiona
-00001630: 6c72 0800 0000 723e 0000 0072 4400 0000  lr....r>...rD...
-00001640: da05 6279 7465 7372 3900 0000 720d 0000  ..bytesr9...r...
-00001650: 0072 5400 0000 7258 0000 0072 2800 0000  .rT...rX...r(...
-00001660: 7228 0000 0072 2800 0000 7229 0000 0072  r(...r(...r)...r
-00001670: 2a00 0000 2300 0000 7374 0000 000a 020e  *...#...st......
-00001680: 0104 0106 0106 0108 0108 0108 0108 010a  ................
-00001690: 010c 010c 0108 0110 0110 0110 0110 010c  ................
-000016a0: f10e 1108 0108 0108 0108 0108 0108 010c  ................
-000016b0: 010c 010c 0108 0110 0110 0110 0110 010c  ................
-000016c0: 0202 0502 0102 fb02 0202 0102 0108 0102  ................
-000016d0: 0108 fa0e 1002 0502 0102 fb02 0202 0106  ................
-000016e0: 0108 0102 010c fa0e 1202 0112 2a0e 1302  ............*...
-000016f0: 0172 2a00 0000 291a 725b 0000 00da 0b64  .r*...).r[.....d
-00001700: 6174 6163 6c61 7373 6573 7202 0000 005a  ataclassesr....Z
-00001710: 0f62 6f72 7368 5f63 6f6e 7374 7275 6374  .borsh_construct
-00001720: 725d 0000 005a 1861 6e63 686f 7270 792e  r]...Z.anchorpy.
-00001730: 626f 7273 685f 6578 7465 6e73 696f 6e72  borsh_extensionr
-00001740: 0300 0000 5a17 616e 6368 6f72 7079 2e63  ....Z.anchorpy.c
-00001750: 6f64 6572 2e61 6363 6f75 6e74 7372 0400  oder.accountsr..
-00001760: 0000 5a0e 616e 6368 6f72 7079 2e65 7272  ..Z.anchorpy.err
-00001770: 6f72 7205 0000 005a 1261 6e63 686f 7270  orr....Z.anchorp
-00001780: 792e 7574 696c 732e 7270 6372 0600 0000  y.utils.rpcr....
-00001790: da14 736f 6c61 6e61 2e72 7063 2e61 7379  ..solana.rpc.asy
-000017a0: 6e63 5f61 7069 7207 0000 00da 1573 6f6c  nc_apir......sol
-000017b0: 616e 612e 7270 632e 636f 6d6d 6974 6d65  ana.rpc.commitme
-000017c0: 6e74 7208 0000 00da 0e73 6f6c 6465 7273  ntr......solders
-000017d0: 2e70 7562 6b65 7972 0900 0000 da00 720b  .pubkeyr......r.
-000017e0: 0000 0072 3200 0000 720c 0000 00da 0954  ...r2...r......T
-000017f0: 7970 6564 4469 6374 720d 0000 0072 2a00  ypedDictr....r*.
-00001800: 0000 7228 0000 0072 2800 0000 7228 0000  ..r(...r(...r(..
-00001810: 0072 2900 0000 da08 3c6d 6f64 756c 653e  .r).....<module>
-00001820: 0100 0000 731c 0000 0008 010c 0208 010c  ....s...........
-00001830: 010c 010c 010c 010c 010c 010c 020c 010c  ................
-00001840: 0312 1202 01                             .....
+00000530: 6507 6a0a 1b00 6405 6507 6a0b 1b00 6406  e.j...d.e.j...d.
+00000540: 6507 6a0c 1b00 6407 6507 6a0a 6408 1900  e.j...d.e.j.d...
+00000550: 1b00 6409 6507 6a0b 640a 1900 1b00 640b  ..d.e.j.d.....d.
+00000560: 6507 6a0b 1b00 640c 650d 6a0e 6a0f 6a10  e.j...d.e.j.j.j.
+00000570: 640d 1900 1b00 640e 650d 6a0e 6a0f 6a10  d.....d.e.j.j.j.
+00000580: 640f 1900 1b00 6410 650d 6a0e 6a0f 6a10  d.....d.e.j.j.j.
+00000590: 1b00 6411 6507 6a11 1b00 6412 650d 6a12  ..d.e.j...d.e.j.
+000005a0: 6a10 1b00 6413 650d 6a13 6a10 1b00 6414  j...d.e.j.j...d.
+000005b0: 650d 6a14 6a15 6a10 1b00 6415 6509 1b00  e.j.j.j...d.e...
+000005c0: 6416 6507 6a0a 6417 1900 1b00 a110 5a10  d.e.j.d.......Z.
+000005d0: 6504 6a05 6506 6418 3c00 6516 6506 6403  e.j.e.d.<.e.e.d.
+000005e0: 3c00 6517 6506 6404 3c00 6517 6506 6405  <.e.e.d.<.e.e.d.
+000005f0: 3c00 6518 6506 6406 3c00 6519 6517 1900  <.e.e.d.<.e.e...
+00000600: 6506 6407 3c00 6519 6517 1900 6506 6409  e.d.<.e.e...e.d.
+00000610: 3c00 6517 6506 640b 3c00 6519 650d 6a0e  <.e.e.d.<.e.e.j.
+00000620: 6a0f 1900 6506 640c 3c00 6519 650d 6a0e  j...e.d.<.e.e.j.
+00000630: 6a0f 1900 6506 640e 3c00 650d 6a0e 6a0f  j...e.d.<.e.j.j.
+00000640: 6506 6410 3c00 6517 6506 6411 3c00 650d  e.d.<.e.e.d.<.e.
+00000650: 6a12 6a1a 6506 6412 3c00 650d 6a13 6a1b  j.j.e.d.<.e.j.j.
+00000660: 6506 6413 3c00 650d 6a14 6a15 6506 6414  e.d.<.e.j.j.e.d.
+00000670: 3c00 6516 6506 6415 3c00 6519 6517 1900  <.e.e.d.<.e.e...
+00000680: 6506 6416 3c00 651c 6419 651d 6602 651e  e.d.<.e.d.e.f.e.
+00000690: 6516 6504 6a1f 6520 1900 6516 6504 6a1f  e.e.j.e ..e.e.j.
+000006a0: 6400 1900 641a 9c05 641b 641c 8405 8301  d...d...d.d.....
+000006b0: 5a21 651c 6419 651d 6602 651e 6519 6516  Z!e.d.e.f.e.e.e.
+000006c0: 1900 6504 6a1f 6520 1900 6516 6504 6a22  ..e.j.e ..e.e.j"
+000006d0: 6504 6a1f 6400 1900 1900 641d 9c05 641e  e.j.d.....d...d.
+000006e0: 641f 8405 8301 5a23 651c 6524 6400 6420  d.....Z#e.e$d.d 
+000006f0: 9c02 6421 6422 8404 8301 5a25 6526 6423  ..d!d"....Z%e&d#
+00000700: 9c01 6424 6425 8404 5a27 651c 6526 6400  ..d$d%..Z'e.e&d.
+00000710: 6426 9c02 6427 6428 8404 8301 5a28 6419  d&..d'd(....Z(d.
+00000720: 5300 2929 da0d 4d61 7267 696e 4163 636f  S.))..MarginAcco
+00000730: 756e 7473 0800 0000 85dc add5 b3d3 2bee  unts..........+.
+00000740: da0d 6469 7363 7269 6d69 6e61 746f 7272  ..discriminatorr
+00000750: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
+00000760: 0000 0072 1200 0000 e98a 0000 0072 1300  ...r.........r..
+00000770: 0000 e905 0000 0072 1400 0000 7215 0000  .......r....r...
+00000780: 00e9 2e00 0000 7216 0000 00e9 5b00 0000  ......r.....[...
+00000790: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+000007a0: 1a00 0000 721b 0000 0072 1c00 0000 721d  ....r....r....r.
+000007b0: 0000 0069 5201 0000 da06 6c61 796f 7574  ...iR.....layout
+000007c0: 4e29 05da 0463 6f6e 6eda 0761 6464 7265  N)...conn..addre
+000007d0: 7373 da0a 636f 6d6d 6974 6d65 6e74 da0a  ss..commitment..
+000007e0: 7072 6f67 7261 6d5f 6964 da06 7265 7475  program_id..retu
+000007f0: 726e 6305 0000 0000 0000 0000 0000 0008  rnc.............
+00000800: 0000 0004 0000 00c3 0000 0073 4800 0000  ...........sH...
+00000810: 7c01 6a00 7c02 7c03 6401 8d02 4900 6400  |.j.|.|.d...I.d.
+00000820: 4800 7d05 7c05 6a01 7d06 7c06 6400 7500  H.}.|.j.}.|.d.u.
+00000830: 7226 6400 5300 7c06 6a02 7c04 6b03 7238  r&d.S.|.j.|.k.r8
+00000840: 7403 6402 8301 8201 7c06 6a04 7d07 7c00  t.d.....|.j.}.|.
+00000850: a005 7c07 a101 5300 a903 4e29 0172 3800  ..|...S...N).r8.
+00000860: 0000 7a27 4163 636f 756e 7420 646f 6573  ..z'Account does
+00000870: 206e 6f74 2062 656c 6f6e 6720 746f 2074   not belong to t
+00000880: 6869 7320 7072 6f67 7261 6d29 06da 1067  his program)...g
+00000890: 6574 5f61 6363 6f75 6e74 5f69 6e66 6fda  et_account_info.
+000008a0: 0576 616c 7565 da05 6f77 6e65 72da 0a56  .value..owner..V
+000008b0: 616c 7565 4572 726f 72da 0464 6174 61da  alueError..data.
+000008c0: 0664 6563 6f64 6529 08da 0363 6c73 7236  .decode)...clsr6
+000008d0: 0000 0072 3700 0000 7238 0000 0072 3900  ...r7...r8...r9.
+000008e0: 0000 da04 7265 7370 da04 696e 666f da0a  ....resp..info..
+000008f0: 6279 7465 735f 6461 7461 722d 0000 0072  bytes_datar-...r
+00000900: 2d00 0000 722e 0000 00da 0566 6574 6368  -...r......fetch
+00000910: 4a00 0000 7310 0000 0000 0814 0106 0108  J...s...........
+00000920: 0104 010a 0108 0106 017a 134d 6172 6769  .........z.Margi
+00000930: 6e41 6363 6f75 6e74 2e66 6574 6368 2905  nAccount.fetch).
+00000940: 7236 0000 00da 0961 6464 7265 7373 6573  r6.....addresses
+00000950: 7238 0000 0072 3900 0000 723a 0000 0063  r8...r9...r:...c
+00000960: 0500 0000 0000 0000 0000 0000 0800 0000  ................
+00000970: 0600 0000 c300 0000 7362 0000 0074 007c  ........sb...t.|
+00000980: 017c 027c 0364 018d 0349 0064 0048 007d  .|.|.d...I.d.H.}
+00000990: 0567 007d 067c 0544 005d 407d 077c 0764  .g.}.|.D.]@}.|.d
+000009a0: 0075 0072 347c 06a0 0164 00a1 0101 0071  .u.r4|...d.....q
+000009b0: 1c7c 076a 026a 037c 046b 0372 4874 0464  .|.j.j.|.k.rHt.d
+000009c0: 0283 0182 017c 06a0 017c 00a0 057c 076a  .....|...|...|.j
+000009d0: 026a 06a1 01a1 0101 0071 1c7c 0653 0072  .j.......q.|.S.r
+000009e0: 3b00 0000 2907 7206 0000 00da 0661 7070  ;...).r......app
+000009f0: 656e 64da 0761 6363 6f75 6e74 723e 0000  end..accountr>..
+00000a00: 0072 3f00 0000 7241 0000 0072 4000 0000  .r?...rA...r@...
+00000a10: 2908 7242 0000 0072 3600 0000 7247 0000  ).rB...r6...rG..
+00000a20: 0072 3800 0000 7239 0000 00da 0569 6e66  .r8...r9.....inf
+00000a30: 6f73 da03 7265 7372 4400 0000 722d 0000  os..resrD...r-..
+00000a40: 0072 2d00 0000 722e 0000 00da 0e66 6574  .r-...r......fet
+00000a50: 6368 5f6d 756c 7469 706c 655b 0000 0073  ch_multiple[...s
+00000a60: 1400 0000 0008 1401 0401 0801 0801 0a01  ................
+00000a70: 0201 0c01 0801 1601 7a1c 4d61 7267 696e  ........z.Margin
+00000a80: 4163 636f 756e 742e 6665 7463 685f 6d75  Account.fetch_mu
+00000a90: 6c74 6970 6c65 2902 7240 0000 0072 3a00  ltiple).r@...r:.
+00000aa0: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
+00000ab0: 0000 0012 0000 0043 0000 0073 b600 0000  .......C...s....
+00000ac0: 7c01 6400 7400 8502 1900 7c00 6a01 6b03  |.d.t.....|.j.k.
+00000ad0: 721a 7402 6401 8301 8201 7403 6a04 a005  r.t.d.....t.j...
+00000ae0: 7c01 7400 6400 8502 1900 a101 7d02 7c00  |.t.d.......}.|.
+00000af0: 7c02 6a06 7c02 6a07 7c02 6a08 7c02 6a09  |.j.|.j.|.j.|.j.
+00000b00: 7c02 6a0a 7c02 6a0b 7c02 6a0c 740d 740e  |.j.|.j.|.j.t.t.
+00000b10: 6402 6403 8400 7c02 6a0f 8302 8301 740d  d.d...|.j.....t.
+00000b20: 740e 6404 6403 8400 7c02 6a10 8302 8301  t.d.d...|.j.....
+00000b30: 7411 6a12 6a13 a014 7c02 6a15 a101 7c02  t.j.j...|.j...|.
+00000b40: 6a16 7411 6a17 a014 7c02 6a17 a101 7411  j.t.j...|.j...t.
+00000b50: 6a18 a014 7c02 6a19 a101 7411 6a1a 6a1b  j...|.j...t.j.j.
+00000b60: a014 7c02 6a1c a101 7c02 6a1d 7c02 6a1e  ..|.j...|.j.|.j.
+00000b70: 6405 8d10 5300 2906 4e7a 2d54 6865 2064  d...S.).Nz-The d
+00000b80: 6973 6372 696d 696e 6174 6f72 2066 6f72  iscriminator for
+00000b90: 2074 6869 7320 6163 636f 756e 7420 6973   this account is
+00000ba0: 2069 6e76 616c 6964 6301 0000 0000 0000   invalidc.......
+00000bb0: 0000 0000 0001 0000 0003 0000 0053 0000  .............S..
+00000bc0: 0073 0e00 0000 7400 6a01 6a02 a003 7c00  .s....t.j.j...|.
+00000bd0: a101 5300 a901 4ea9 0472 0b00 0000 7226  ..S...N..r....r&
+00000be0: 0000 00da 0d50 726f 6475 6374 4c65 6467  .....ProductLedg
+00000bf0: 6572 da0c 6672 6f6d 5f64 6563 6f64 6564  er..from_decoded
+00000c00: a901 da04 6974 656d 722d 0000 0072 2d00  ....itemr-...r-.
+00000c10: 0000 722e 0000 00da 083c 6c61 6d62 6461  ..r......<lambda
+00000c20: 3e7d 0000 00f3 0000 0000 7a26 4d61 7267  >}........z&Marg
+00000c30: 696e 4163 636f 756e 742e 6465 636f 6465  inAccount.decode
+00000c40: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+00000c50: 613e 6301 0000 0000 0000 0000 0000 0001  a>c.............
+00000c60: 0000 0003 0000 0053 0000 0073 0e00 0000  .......S...s....
+00000c70: 7400 6a01 6a02 a003 7c00 a101 5300 724d  t.j.j...|...S.rM
+00000c80: 0000 0072 4e00 0000 7251 0000 0072 2d00  ...rN...rQ...r-.
+00000c90: 0000 722d 0000 0072 2e00 0000 7253 0000  ..r-...r....rS..
+00000ca0: 0083 0000 0072 5400 0000 a910 720e 0000  .....rT.....r...
+00000cb0: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
+00000cc0: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+00000cd0: 1500 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
+00000ce0: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
+00000cf0: 0000 721c 0000 0072 1d00 0000 291f 7204  ..r....r....).r.
+00000d00: 0000 0072 3000 0000 7205 0000 0072 2f00  ...r0...r....r/.
+00000d10: 0000 7235 0000 00da 0570 6172 7365 720e  ..r5.....parser.
+00000d20: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
+00000d30: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00000d40: 0072 2500 0000 da03 6d61 7072 1500 0000  .r%.....mapr....
+00000d50: 7216 0000 0072 0b00 0000 7226 0000 0072  r....r....r&...r
+00000d60: 4f00 0000 7250 0000 0072 1700 0000 7218  O...rP...r....r.
+00000d70: 0000 0072 1900 0000 7229 0000 0072 1a00  ...r....r)...r..
+00000d80: 0000 722b 0000 00da 0d41 6e63 686f 7244  ..r+.....AnchorD
+00000d90: 6563 696d 616c 721b 0000 0072 1c00 0000  ecimalr....r....
+00000da0: 721d 0000 0029 0372 4200 0000 7240 0000  r....).rB...r@..
+00000db0: 00da 0364 6563 722d 0000 0072 2d00 0000  ...decr-...r-...
+00000dc0: 722e 0000 0072 4100 0000 6e00 0000 733e  r....rA...n...s>
+00000dd0: 0000 0000 0212 0108 0114 0102 0104 0104  ................
+00000de0: 0104 0104 0104 0104 0104 0102 0102 0106  ................
+00000df0: 0104 fe02 ff02 0602 0102 0106 0104 fe02  ................
+00000e00: ff02 060e 0104 010c 010c 010e 0104 0104  ................
+00000e10: e67a 144d 6172 6769 6e41 6363 6f75 6e74  .z.MarginAccount
+00000e20: 2e64 6563 6f64 6529 0172 3a00 0000 6301  .decode).r:...c.
+00000e30: 0000 0000 0000 0000 0000 0001 0000 0011  ................
+00000e40: 0000 0043 0000 0073 7a00 0000 7400 7c00  ...C...sz...t.|.
+00000e50: 6a01 8301 7c00 6a02 7c00 6a03 7c00 6a04  j...|.j.|.j.|.j.
+00000e60: 7c00 6a05 7c00 6a06 7c00 6a07 7408 7409  |.j.|.j.|.j.t.t.
+00000e70: 6401 6402 8400 7c00 6a0a 8302 8301 7408  d.d...|.j.....t.
+00000e80: 7409 6403 6402 8400 7c00 6a0b 8302 8301  t.d.d...|.j.....
+00000e90: 7c00 6a0c a00d a100 7c00 6a0e 7c00 6a0f  |.j.....|.j.|.j.
+00000ea0: a00d a100 7c00 6a10 a00d a100 7c00 6a11  ....|.j.....|.j.
+00000eb0: a00d a100 7400 7c00 6a12 8301 7c00 6a13  ....t.|.j...|.j.
+00000ec0: 6404 9c10 5300 2905 4e63 0100 0000 0000  d...S.).Nc......
+00000ed0: 0000 0000 0000 0100 0000 0200 0000 5300  ..............S.
+00000ee0: 0000 7308 0000 007c 00a0 00a1 0053 0072  ..s....|.....S.r
+00000ef0: 4d00 0000 a901 da07 746f 5f6a 736f 6e72  M.......to_jsonr
+00000f00: 5100 0000 722d 0000 0072 2d00 0000 722e  Q...r-...r-...r.
+00000f10: 0000 0072 5300 0000 9900 0000 7254 0000  ...rS.......rT..
+00000f20: 007a 274d 6172 6769 6e41 6363 6f75 6e74  .z'MarginAccount
+00000f30: 2e74 6f5f 6a73 6f6e 2e3c 6c6f 6361 6c73  .to_json.<locals
+00000f40: 3e2e 3c6c 616d 6264 613e 6301 0000 0000  >.<lambda>c.....
+00000f50: 0000 0000 0000 0001 0000 0002 0000 0053  ...............S
+00000f60: 0000 0073 0800 0000 7c00 a000 a100 5300  ...s....|.....S.
+00000f70: 724d 0000 0072 5a00 0000 7251 0000 0072  rM...rZ...rQ...r
+00000f80: 2d00 0000 722d 0000 0072 2e00 0000 7253  -...r-...r....rS
+00000f90: 0000 009a 0000 0072 5400 0000 7255 0000  .......rT...rU..
+00000fa0: 0029 1472 2100 0000 720e 0000 0072 0f00  .).r!...r....r..
+00000fb0: 0000 7210 0000 0072 1100 0000 7212 0000  ..r....r....r...
+00000fc0: 0072 1300 0000 7214 0000 0072 2500 0000  .r....r....r%...
+00000fd0: 7257 0000 0072 1500 0000 7216 0000 0072  rW...r....r....r
+00000fe0: 1700 0000 725b 0000 0072 1800 0000 7219  ....r[...r....r.
+00000ff0: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
+00001000: 0000 721d 0000 0029 01da 0473 656c 6672  ..r....)...selfr
+00001010: 2d00 0000 722d 0000 0072 2e00 0000 725b  -...r-...r....r[
+00001020: 0000 0090 0000 0073 2200 0000 0002 0801  .......s".......
+00001030: 0401 0401 0401 0401 0401 0401 1201 1201  ................
+00001040: 0801 0401 0801 0801 0801 0801 04f0 7a15  ..............z.
+00001050: 4d61 7267 696e 4163 636f 756e 742e 746f  MarginAccount.to
+00001060: 5f6a 736f 6e29 02da 036f 626a 723a 0000  _json)...objr:..
+00001070: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+00001080: 0000 1300 0000 4300 0000 73b4 0000 007c  ......C...s....|
+00001090: 0074 00a0 017c 0164 0119 00a1 017c 0164  .t...|.d.....|.d
+000010a0: 0219 007c 0164 0319 007c 0164 0419 007c  ...|.d...|.d...|
+000010b0: 0164 0519 007c 0164 0619 007c 0164 0719  .d...|.d...|.d..
+000010c0: 0074 0274 0364 0864 0984 007c 0164 0a19  .t.t.d.d...|.d..
+000010d0: 0083 0283 0174 0274 0364 0b64 0984 007c  .....t.t.d.d...|
+000010e0: 0164 0c19 0083 0283 0174 046a 056a 06a0  .d.......t.j.j..
+000010f0: 077c 0164 0d19 00a1 017c 0164 0e19 0074  .|.d.....|.d...t
+00001100: 046a 08a0 077c 0164 0f19 00a1 0174 046a  .j...|.d.....t.j
+00001110: 09a0 077c 0164 1019 00a1 0174 046a 0a6a  ...|.d.....t.j.j
+00001120: 0ba0 077c 0164 1119 00a1 0174 00a0 017c  ...|.d.....t...|
+00001130: 0164 1219 00a1 017c 0164 1319 0064 148d  .d.....|.d...d..
+00001140: 1053 0029 154e 720e 0000 0072 0f00 0000  .S.).Nr....r....
+00001150: 7210 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00001160: 1300 0000 7214 0000 0063 0100 0000 0000  ....r....c......
+00001170: 0000 0000 0000 0100 0000 0300 0000 5300  ..............S.
+00001180: 0000 730e 0000 0074 006a 016a 02a0 037c  ..s....t.j.j...|
+00001190: 00a1 0153 0072 4d00 0000 a904 720b 0000  ...S.rM.....r...
+000011a0: 0072 2600 0000 724f 0000 00da 0966 726f  .r&...rO.....fro
+000011b0: 6d5f 6a73 6f6e 7251 0000 0072 2d00 0000  m_jsonrQ...r-...
+000011c0: 722d 0000 0072 2e00 0000 7253 0000 00b0  r-...r....rS....
+000011d0: 0000 0072 5400 0000 7a29 4d61 7267 696e  ...rT...z)Margin
+000011e0: 4163 636f 756e 742e 6672 6f6d 5f6a 736f  Account.from_jso
+000011f0: 6e2e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  n.<locals>.<lamb
+00001200: 6461 3e72 1500 0000 6301 0000 0000 0000  da>r....c.......
+00001210: 0000 0000 0001 0000 0003 0000 0053 0000  .............S..
+00001220: 0073 0e00 0000 7400 6a01 6a02 a003 7c00  .s....t.j.j...|.
+00001230: a101 5300 724d 0000 0072 5e00 0000 7251  ..S.rM...r^...rQ
+00001240: 0000 0072 2d00 0000 722d 0000 0072 2e00  ...r-...r-...r..
+00001250: 0000 7253 0000 00b6 0000 0072 5400 0000  ..rS.......rT...
+00001260: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00001270: 1900 0000 721a 0000 0072 1b00 0000 721c  ....r....r....r.
+00001280: 0000 0072 1d00 0000 7255 0000 0029 0c72  ...r....rU...).r
+00001290: 0900 0000 da0b 6672 6f6d 5f73 7472 696e  ......from_strin
+000012a0: 6772 2500 0000 7257 0000 0072 0b00 0000  gr%...rW...r....
+000012b0: 7226 0000 0072 4f00 0000 725f 0000 0072  r&...rO...r_...r
+000012c0: 1900 0000 7229 0000 0072 2b00 0000 7258  ....r)...r+...rX
+000012d0: 0000 0029 0272 4200 0000 725d 0000 0072  ...).rB...r]...r
+000012e0: 2d00 0000 722d 0000 0072 2e00 0000 725f  -...r-...r....r_
+000012f0: 0000 00a4 0000 0073 3800 0000 0002 0201  .......s8.......
+00001300: 0c01 0601 0601 0601 0601 0601 0601 0201  ................
+00001310: 0201 0601 06fe 02ff 0206 0201 0201 0601  ................
+00001320: 06fe 02ff 0206 1001 0601 0e01 0e01 1001  ................
+00001330: 0c01 06e6 7a17 4d61 7267 696e 4163 636f  ....z.MarginAcco
+00001340: 756e 742e 6672 6f6d 5f6a 736f 6e29 2972  unt.from_json))r
+00001350: 1e00 0000 721f 0000 0072 2000 0000 7230  ....r....r ...r0
+00001360: 0000 00da 0674 7970 696e 67da 0843 6c61  .....typing..Cla
+00001370: 7373 5661 7272 2200 0000 da05 626f 7273  ssVarr".....bors
+00001380: 68da 0743 5374 7275 6374 7203 0000 00da  h..CStructr.....
+00001390: 0255 38da 0355 3634 da04 426f 6f6c 720b  .U8..U64..Boolr.
+000013a0: 0000 0072 2600 0000 724f 0000 0072 3500  ...r&...rO...r5.
+000013b0: 0000 da03 4936 3472 1900 0000 7229 0000  ....I64r....r)..
+000013c0: 0072 2b00 0000 7258 0000 0072 0900 0000  .r+...rX...r....
+000013d0: 7223 0000 0072 2400 0000 7225 0000 00da  r#...r$...r%....
+000013e0: 0941 7373 6574 4b69 6e64 da15 4d61 7267  .AssetKind..Marg
+000013f0: 696e 4163 636f 756e 7454 7970 654b 696e  inAccountTypeKin
+00001400: 64da 0b63 6c61 7373 6d65 7468 6f64 720c  d..classmethodr.
+00001410: 0000 0072 0700 0000 da08 4f70 7469 6f6e  ...r......Option
+00001420: 616c 7208 0000 0072 4600 0000 da04 4c69  alr....rF.....Li
+00001430: 7374 724c 0000 00da 0562 7974 6573 7241  strL.....bytesrA
+00001440: 0000 0072 0d00 0000 725b 0000 0072 5f00  ...r....r[...r_.
+00001450: 0000 722d 0000 0072 2d00 0000 722d 0000  ..r-...r-...r-..
+00001460: 0072 2e00 0000 722f 0000 0024 0000 0073  .r....r/...$...s
+00001470: 7800 0000 0a02 0e01 0401 0601 0801 0801  x...............
+00001480: 0801 0c01 0c01 0801 1001 1001 0c01 0801  ................
+00001490: 0a01 0a01 0c01 0601 0cf0 0e12 0801 0801  ................
+000014a0: 0801 0801 0c01 0c01 0801 1001 1001 0c01  ................
+000014b0: 0801 0c01 0c01 0c01 0801 0c02 0205 0201  ................
+000014c0: 02fb 0202 0201 0201 0801 0201 08fa 0e10  ................
+000014d0: 0205 0201 02fb 0202 0201 0601 0801 0201  ................
+000014e0: 0efa 0e12 0201 1221 0e14 0201 722f 0000  .......!....r/..
+000014f0: 0029 1a72 6100 0000 da0b 6461 7461 636c  .).ra.....datacl
+00001500: 6173 7365 7372 0200 0000 da0f 626f 7273  assesr......bors
+00001510: 685f 636f 6e73 7472 7563 7472 6300 0000  h_constructrc...
+00001520: da18 616e 6368 6f72 7079 2e62 6f72 7368  ..anchorpy.borsh
+00001530: 5f65 7874 656e 7369 6f6e 7203 0000 00da  _extensionr.....
+00001540: 1761 6e63 686f 7270 792e 636f 6465 722e  .anchorpy.coder.
+00001550: 6163 636f 756e 7473 7204 0000 005a 0e61  accountsr....Z.a
+00001560: 6e63 686f 7270 792e 6572 726f 7272 0500  nchorpy.errorr..
+00001570: 0000 5a12 616e 6368 6f72 7079 2e75 7469  ..Z.anchorpy.uti
+00001580: 6c73 2e72 7063 7206 0000 00da 1473 6f6c  ls.rpcr......sol
+00001590: 616e 612e 7270 632e 6173 796e 635f 6170  ana.rpc.async_ap
+000015a0: 6972 0700 0000 da15 736f 6c61 6e61 2e72  ir......solana.r
+000015b0: 7063 2e63 6f6d 6d69 746d 656e 7472 0800  pc.commitmentr..
+000015c0: 0000 da0e 736f 6c64 6572 732e 7075 626b  ....solders.pubk
+000015d0: 6579 7209 0000 00da 0072 0b00 0000 7239  eyr......r....r9
+000015e0: 0000 0072 0c00 0000 da09 5479 7065 6444  ...r......TypedD
+000015f0: 6963 7472 0d00 0000 722f 0000 0072 2d00  ictr....r/...r-.
+00001600: 0000 722d 0000 0072 2d00 0000 722e 0000  ..r-...r-...r...
+00001610: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00001620: 1c00 0000 0801 0c02 0801 0c01 0c01 0c01  ................
+00001630: 0c01 0c01 0c01 0c02 0c01 0c03 1213 0201  ................
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/cross_margin_account_manager.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/cross_margin_account_manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/cross_margin_account_manager.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/cross_margin_account_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/cross_open_orders_map.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/cross_open_orders_map.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/cross_open_orders_map.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/cross_open_orders_map.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/greeks.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/greeks.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/greeks.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/greeks.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/insurance_deposit_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/insurance_deposit_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/insurance_deposit_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/insurance_deposit_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/margin_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/margin_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/market_indexes.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/market_indexes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/market_indexes.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/market_indexes.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/market_node.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/market_node.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/market_node.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/market_node.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/open_orders_map.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/open_orders_map.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/open_orders_map.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/open_orders_map.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/perp_sync_queue.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/perp_sync_queue.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/perp_sync_queue.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/perp_sync_queue.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/pricing.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/pricing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/pricing.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/pricing.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Sep 12 11:00:06 2023 UTC, .py size: 17452 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b644 0065 2c44 0000  a........D.e,D..
+00000000: 610d 0d0a 0000 0000 ae9a 6865 2c44 0000  a.........he,D..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a04 6400 6403 6c05  ..d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6400 6407 6c0d  d.l.m.Z...d.d.l.
@@ -103,649 +103,650 @@
 00000660: 696d 616c da11 416e 6368 6f72 4465 6369  imal..AnchorDeci
 00000670: 6d61 6c4a 534f 4eda 0373 7472 7221 0000  malJSON..strr!..
 00000680: 00da 1250 6572 7050 6172 616d 6574 6572  ...PerpParameter
 00000690: 734a 534f 4e72 2300 0000 da14 4d61 7267  sJSONr#.....Marg
 000006a0: 696e 5061 7261 6d65 7465 7273 4a53 4f4e  inParametersJSON
 000006b0: da07 7072 6f64 7563 74da 0b50 726f 6475  ..product..Produ
 000006c0: 6374 4a53 4f4e da04 626f 6f6c a900 723d  ctJSON..bool..r=
-000006d0: 0000 0072 3d00 0000 fa4d 2f55 7365 7273  ...r=....M/Users
+000006d0: 0000 0072 3d00 0000 fa5b 2f55 7365 7273  ...r=....[/Users
 000006e0: 2f74 6672 697a 7a61 2f44 6f63 756d 656e  /tfrizza/Documen
-000006f0: 7473 2f7a 6574 612f 7a65 7461 2d70 792f  ts/zeta/zeta-py/
-00000700: 7a65 7461 5f70 792f 7a65 7461 5f63 6c69  zeta_py/zeta_cli
-00000710: 656e 742f 6163 636f 756e 7473 2f70 7269  ent/accounts/pri
-00000720: 6369 6e67 2e70 7972 0d00 0000 1100 0000  cing.pyr........
-00000730: 7342 0000 000a 0108 010c 010c 010c 010c  sB..............
-00000740: 0110 0110 0110 0110 010c 010c 010c 010c  ................
-00000750: 010c 010c 010c 010c 010c 010c 0110 0110  ................
-00000760: 0110 0110 0110 0110 010c 010c 0108 0108  ................
-00000770: 0108 010c 010c 0172 0d00 0000 6300 0000  .......r....c...
-00000780: 0000 0000 0000 0000 0000 0000 0025 0000  .............%..
-00000790: 0040 0000 0073 fa03 0000 6500 5a01 6400  .@...s....e.Z.d.
-000007a0: 5a02 5500 6401 5a03 6504 6a05 6506 6402  Z.U.d.Z.e.j.e.d.
-000007b0: 3c00 6507 a008 6403 6507 6a09 1b00 6404  <.e...d.e.j...d.
-000007c0: 6507 6a0a 6405 1900 1b00 6406 6507 6a0a  e.j.d.....d.e.j.
-000007d0: 6407 1900 1b00 6408 6507 6a0a 6405 1900  d.....d.e.j.d...
-000007e0: 1b00 6409 6507 6a0a 6407 1900 1b00 640a  ..d.e.j.d.....d.
-000007f0: 650b 6a0c 6a0d 6a0e 6405 1900 1b00 640b  e.j.j.j.d.....d.
-00000800: 650b 6a0c 6a0d 6a0e 6407 1900 1b00 640c  e.j.j.j.d.....d.
-00000810: 650b 6a0c 6a0d 6a0e 6405 1900 1b00 640d  e.j.j.j.d.....d.
-00000820: 650b 6a0c 6a0d 6a0e 6407 1900 1b00 640e  e.j.j.j.d.....d.
-00000830: 6507 6a0a 6405 1900 1b00 640f 6507 6a0a  e.j.d.....d.e.j.
-00000840: 6407 1900 1b00 6410 650f 6405 1900 1b00  d.....d.e.d.....
-00000850: 6411 650f 6407 1900 1b00 6412 650f 6405  d.e.d.....d.e.d.
-00000860: 1900 1b00 6413 650f 6407 1900 1b00 6414  ....d.e.d.....d.
-00000870: 650f 6405 1900 1b00 6415 650f 6407 1900  e.d.....d.e.d...
-00000880: 1b00 6416 650f 6405 1900 1b00 6417 650f  ..d.e.d.....d.e.
-00000890: 6407 1900 1b00 6418 650b 6a10 6a11 6a0e  d.....d.e.j.j.j.
-000008a0: 6405 1900 1b00 6419 650b 6a10 6a11 6a0e  d.....d.e.j.j.j.
-000008b0: 6407 1900 1b00 641a 650b 6a12 6a13 6a0e  d.....d.e.j.j.j.
-000008c0: 6405 1900 1b00 641b 650b 6a12 6a13 6a0e  d.....d.e.j.j.j.
-000008d0: 6407 1900 1b00 641c 650b 6a14 6a15 6a0e  d.....d.e.j.j.j.
-000008e0: 6405 1900 1b00 641d 650b 6a14 6a15 6a0e  d.....d.e.j.j.j.
-000008f0: 6407 1900 1b00 641e 650f 6405 1900 1b00  d.....d.e.d.....
-00000900: 641f 650f 6407 1900 1b00 6420 6507 6a0a  d.e.d.....d e.j.
-00000910: 1b00 6421 6507 6a0a 1b00 6422 6507 6a16  ..d!e.j...d"e.j.
-00000920: 1b00 6423 6507 6a17 6405 1900 1b00 6424  ..d#e.j.d.....d$
-00000930: 6507 6a17 6407 1900 1b00 6425 6507 6a09  e.j.d.....d%e.j.
-00000940: 6426 1900 1b00 a121 5a0e 6504 6a05 6506  d&.....!Z.e.j.e.
-00000950: 6427 3c00 6518 6506 6403 3c00 6519 6518  d'<.e.e.d.<.e.e.
-00000960: 1900 6506 6404 3c00 6519 6518 1900 6506  ..e.d.<.e.e...e.
-00000970: 6406 3c00 6519 6518 1900 6506 6408 3c00  d.<.e.e...e.d.<.
-00000980: 6519 6518 1900 6506 6409 3c00 6519 650b  e.e...e.d.<.e.e.
-00000990: 6a0c 6a0d 1900 6506 640a 3c00 6519 650b  j.j...e.d.<.e.e.
-000009a0: 6a0c 6a0d 1900 6506 640b 3c00 6519 650b  j.j...e.d.<.e.e.
-000009b0: 6a0c 6a0d 1900 6506 640c 3c00 6519 650b  j.j...e.d.<.e.e.
-000009c0: 6a0c 6a0d 1900 6506 640d 3c00 6519 6518  j.j...e.d.<.e.e.
-000009d0: 1900 6506 640e 3c00 6519 6518 1900 6506  ..e.d.<.e.e...e.
-000009e0: 640f 3c00 6519 651a 1900 6506 6410 3c00  d.<.e.e...e.d.<.
-000009f0: 6519 651a 1900 6506 6411 3c00 6519 651a  e.e...e.d.<.e.e.
-00000a00: 1900 6506 6412 3c00 6519 651a 1900 6506  ..e.d.<.e.e...e.
-00000a10: 6413 3c00 6519 651a 1900 6506 6414 3c00  d.<.e.e...e.d.<.
-00000a20: 6519 651a 1900 6506 6415 3c00 6519 651a  e.e...e.d.<.e.e.
-00000a30: 1900 6506 6416 3c00 6519 651a 1900 6506  ..e.d.<.e.e...e.
-00000a40: 6417 3c00 6519 650b 6a10 6a11 1900 6506  d.<.e.e.j.j...e.
-00000a50: 6418 3c00 6519 650b 6a10 6a11 1900 6506  d.<.e.e.j.j...e.
-00000a60: 6419 3c00 6519 650b 6a12 6a13 1900 6506  d.<.e.e.j.j...e.
-00000a70: 641a 3c00 6519 650b 6a12 6a13 1900 6506  d.<.e.e.j.j...e.
-00000a80: 641b 3c00 6519 650b 6a14 6a15 1900 6506  d.<.e.e.j.j...e.
-00000a90: 641c 3c00 6519 650b 6a14 6a15 1900 6506  d.<.e.e.j.j...e.
-00000aa0: 641d 3c00 6519 651a 1900 6506 641e 3c00  d.<.e.e...e.d.<.
-00000ab0: 6519 651a 1900 6506 641f 3c00 6518 6506  e.e...e.d.<.e.e.
-00000ac0: 6420 3c00 6518 6506 6421 3c00 6518 6506  d <.e.e.d!<.e.e.
-00000ad0: 6422 3c00 6519 651b 1900 6506 6423 3c00  d"<.e.e...e.d#<.
-00000ae0: 6519 651b 1900 6506 6424 3c00 6519 6518  e.e...e.d$<.e.e.
-00000af0: 1900 6506 6425 3c00 651c 6428 651d 6602  ..e.d%<.e.d(e.f.
-00000b00: 651e 651a 6504 6a1f 6520 1900 651a 6504  e.e.e.j.e ..e.e.
-00000b10: 6a1f 6400 1900 6429 9c05 642a 642b 8405  j.d...d)..d*d+..
-00000b20: 8301 5a21 651c 6428 651d 6602 651e 6519  ..Z!e.d(e.f.e.e.
-00000b30: 651a 1900 6504 6a1f 6520 1900 651a 6504  e...e.j.e ..e.e.
-00000b40: 6a22 6504 6a1f 6400 1900 1900 642c 9c05  j"e.j.d.....d,..
-00000b50: 642d 642e 8405 8301 5a23 651c 6524 6400  d-d.....Z#e.e$d.
-00000b60: 642f 9c02 6430 6431 8404 8301 5a25 6526  d/..d0d1....Z%e&
-00000b70: 6432 9c01 6433 6434 8404 5a27 651c 6526  d2..d3d4..Z'e.e&
-00000b80: 6400 6435 9c02 6436 6437 8404 8301 5a28  d.d5..d6d7....Z(
-00000b90: 6428 5300 2938 da07 5072 6963 696e 6773  d(S.)8..Pricings
-00000ba0: 0800 0000 be7b d2b6 8f0b 9888 da0d 6469  .....{........di
-00000bb0: 7363 7269 6d69 6e61 746f 7272 0e00 0000  scriminatorr....
-00000bc0: 720f 0000 00e9 0500 0000 7210 0000 00e9  r.........r.....
-00000bd0: 1400 0000 7211 0000 0072 1200 0000 7213  ....r....r....r.
-00000be0: 0000 0072 1400 0000 7215 0000 0072 1600  ...r....r....r..
-00000bf0: 0000 7217 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000c00: 0072 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00000c10: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00000c20: 2000 0000 7221 0000 0072 2200 0000 7223   ...r!...r"...r#
-00000c30: 0000 0072 2400 0000 7225 0000 0072 2600  ...r$...r%...r&.
-00000c40: 0000 7227 0000 0072 2800 0000 7229 0000  ..r'...r(...r)..
-00000c50: 0072 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
-00000c60: 722d 0000 0072 2e00 0000 6993 0a00 00da  r-...r....i.....
-00000c70: 066c 6179 6f75 744e 2905 da04 636f 6e6e  .layoutN)...conn
-00000c80: da07 6164 6472 6573 73da 0a63 6f6d 6d69  ..address..commi
-00000c90: 746d 656e 74da 0a70 726f 6772 616d 5f69  tment..program_i
-00000ca0: 64da 0672 6574 7572 6e63 0500 0000 0000  d..returnc......
-00000cb0: 0000 0000 0000 0800 0000 0400 0000 c300  ................
-00000cc0: 0000 7348 0000 007c 016a 007c 027c 0364  ..sH...|.j.|.|.d
-00000cd0: 018d 0249 0064 0048 007d 057c 056a 017d  ...I.d.H.}.|.j.}
-00000ce0: 067c 0664 0075 0072 2664 0053 007c 066a  .|.d.u.r&d.S.|.j
-00000cf0: 027c 046b 0372 3874 0364 0283 0182 017c  .|.k.r8t.d.....|
-00000d00: 066a 047d 077c 00a0 057c 07a1 0153 00a9  .j.}.|...|...S..
-00000d10: 034e 2901 7246 0000 007a 2741 6363 6f75  .N).rF...z'Accou
-00000d20: 6e74 2064 6f65 7320 6e6f 7420 6265 6c6f  nt does not belo
-00000d30: 6e67 2074 6f20 7468 6973 2070 726f 6772  ng to this progr
-00000d40: 616d 2906 da10 6765 745f 6163 636f 756e  am)...get_accoun
-00000d50: 745f 696e 666f da05 7661 6c75 65da 056f  t_info..value..o
-00000d60: 776e 6572 da0a 5661 6c75 6545 7272 6f72  wner..ValueError
-00000d70: da04 6461 7461 da06 6465 636f 6465 2908  ..data..decode).
-00000d80: da03 636c 7372 4400 0000 7245 0000 0072  ..clsrD...rE...r
-00000d90: 4600 0000 7247 0000 00da 0472 6573 70da  F...rG.....resp.
-00000da0: 0469 6e66 6fda 0a62 7974 6573 5f64 6174  .info..bytes_dat
-00000db0: 6172 3d00 0000 723d 0000 0072 3e00 0000  ar=...r=...r>...
-00000dc0: da05 6665 7463 687d 0000 0073 1000 0000  ..fetch}...s....
-00000dd0: 0008 1401 0601 0801 0401 0a01 0801 0601  ................
-00000de0: 7a0d 5072 6963 696e 672e 6665 7463 6829  z.Pricing.fetch)
-00000df0: 0572 4400 0000 da09 6164 6472 6573 7365  .rD.....addresse
-00000e00: 7372 4600 0000 7247 0000 0072 4800 0000  srF...rG...rH...
-00000e10: 6305 0000 0000 0000 0000 0000 0008 0000  c...............
-00000e20: 0006 0000 00c3 0000 0073 6200 0000 7400  .........sb...t.
-00000e30: 7c01 7c02 7c03 6401 8d03 4900 6400 4800  |.|.|.d...I.d.H.
-00000e40: 7d05 6700 7d06 7c05 4400 5d40 7d07 7c07  }.g.}.|.D.]@}.|.
-00000e50: 6400 7500 7234 7c06 a001 6400 a101 0100  d.u.r4|...d.....
-00000e60: 711c 7c07 6a02 6a03 7c04 6b03 7248 7404  q.|.j.j.|.k.rHt.
-00000e70: 6402 8301 8201 7c06 a001 7c00 a005 7c07  d.....|...|...|.
-00000e80: 6a02 6a06 a101 a101 0100 711c 7c06 5300  j.j.......q.|.S.
-00000e90: 7249 0000 0029 0772 0600 0000 da06 6170  rI...).r......ap
-00000ea0: 7065 6e64 da07 6163 636f 756e 7472 4c00  pend..accountrL.
-00000eb0: 0000 724d 0000 0072 4f00 0000 724e 0000  ..rM...rO...rN..
-00000ec0: 0029 0872 5000 0000 7244 0000 0072 5500  .).rP...rD...rU.
-00000ed0: 0000 7246 0000 0072 4700 0000 da05 696e  ..rF...rG.....in
-00000ee0: 666f 73da 0372 6573 7252 0000 0072 3d00  fos..resrR...r=.
-00000ef0: 0000 723d 0000 0072 3e00 0000 da0e 6665  ..r=...r>.....fe
-00000f00: 7463 685f 6d75 6c74 6970 6c65 8e00 0000  tch_multiple....
-00000f10: 7314 0000 0000 0814 0104 0108 0108 010a  s...............
-00000f20: 0102 010c 0108 0116 017a 1650 7269 6369  .........z.Prici
-00000f30: 6e67 2e66 6574 6368 5f6d 756c 7469 706c  ng.fetch_multipl
-00000f40: 6529 0272 4e00 0000 7248 0000 0063 0200  e).rN...rH...c..
-00000f50: 0000 0000 0000 0000 0000 0300 0000 2300  ..............#.
-00000f60: 0000 4300 0000 7346 0100 007c 0164 0074  ..C...sF...|.d.t
-00000f70: 0085 0219 007c 006a 016b 0372 1a74 0264  .....|.j.k.r.t.d
-00000f80: 0183 0182 0174 036a 04a0 057c 0174 0064  .....t.j...|.t.d
-00000f90: 0085 0219 00a1 017d 027c 007c 026a 067c  .......}.|.|.j.|
-00000fa0: 026a 077c 026a 087c 026a 097c 026a 0a74  .j.|.j.|.j.|.j.t
-00000fb0: 0b74 0c64 0264 0384 007c 026a 0d83 0283  .t.d.d...|.j....
-00000fc0: 0174 0b74 0c64 0464 0384 007c 026a 0e83  .t.t.d.d...|.j..
-00000fd0: 0283 0174 0b74 0c64 0564 0384 007c 026a  ...t.t.d.d...|.j
-00000fe0: 0f83 0283 0174 0b74 0c64 0664 0384 007c  .....t.t.d.d...|
-00000ff0: 026a 1083 0283 017c 026a 117c 026a 127c  .j.....|.j.|.j.|
-00001000: 026a 137c 026a 147c 026a 157c 026a 167c  .j.|.j.|.j.|.j.|
-00001010: 026a 177c 026a 187c 026a 197c 026a 1a74  .j.|.j.|.j.|.j.t
-00001020: 0b74 0c64 0764 0384 007c 026a 1b83 0283  .t.d.d...|.j....
-00001030: 0174 0b74 0c64 0864 0384 007c 026a 1c83  .t.t.d.d...|.j..
-00001040: 0283 0174 0b74 0c64 0964 0384 007c 026a  ...t.t.d.d...|.j
-00001050: 1d83 0283 0174 0b74 0c64 0a64 0384 007c  .....t.t.d.d...|
-00001060: 026a 1e83 0283 0174 0b74 0c64 0b64 0384  .j.....t.t.d.d..
-00001070: 007c 026a 1f83 0283 0174 0b74 0c64 0c64  .|.j.....t.t.d.d
-00001080: 0384 007c 026a 2083 0283 017c 026a 217c  ...|.j ....|.j!|
-00001090: 026a 227c 026a 237c 026a 247c 026a 257c  .j"|.j#|.j$|.j%|
-000010a0: 026a 267c 026a 277c 026a 2864 0d8d 2153  .j&|.j'|.j(d..!S
-000010b0: 0029 0e4e 7a2d 5468 6520 6469 7363 7269  .).Nz-The discri
-000010c0: 6d69 6e61 746f 7220 666f 7220 7468 6973  minator for this
-000010d0: 2061 6363 6f75 6e74 2069 7320 696e 7661   account is inva
-000010e0: 6c69 6463 0100 0000 0000 0000 0000 0000  lidc............
-000010f0: 0100 0000 0300 0000 5300 0000 730e 0000  ........S...s...
-00001100: 0074 006a 016a 02a0 037c 00a1 0153 00a9  .t.j.j...|...S..
-00001110: 014e a904 720b 0000 0072 3500 0000 da0d  .N..r....r5.....
-00001120: 416e 6368 6f72 4465 6369 6d61 6cda 0c66  AnchorDecimal..f
-00001130: 726f 6d5f 6465 636f 6465 64a9 01da 0469  rom_decoded....i
-00001140: 7465 6d72 3d00 0000 723d 0000 0072 3e00  temr=...r=...r>.
-00001150: 0000 da08 3c6c 616d 6264 613e ae00 0000  ....<lambda>....
-00001160: f300 0000 007a 2050 7269 6369 6e67 2e64  .....z Pricing.d
-00001170: 6563 6f64 652e 3c6c 6f63 616c 733e 2e3c  ecode.<locals>.<
-00001180: 6c61 6d62 6461 3e63 0100 0000 0000 0000  lambda>c........
-00001190: 0000 0000 0100 0000 0300 0000 5300 0000  ............S...
-000011a0: 730e 0000 0074 006a 016a 02a0 037c 00a1  s....t.j.j...|..
-000011b0: 0153 0072 5b00 0000 725c 0000 0072 5f00  .S.r[...r\...r_.
-000011c0: 0000 723d 0000 0072 3d00 0000 723e 0000  ..r=...r=...r>..
-000011d0: 0072 6100 0000 b400 0000 7262 0000 0063  .ra.......rb...c
-000011e0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000011f0: 0300 0000 5300 0000 730e 0000 0074 006a  ....S...s....t.j
-00001200: 016a 02a0 037c 00a1 0153 0072 5b00 0000  .j...|...S.r[...
-00001210: 725c 0000 0072 5f00 0000 723d 0000 0072  r\...r_...r=...r
-00001220: 3d00 0000 723e 0000 0072 6100 0000 ba00  =...r>...ra.....
-00001230: 0000 7262 0000 0063 0100 0000 0000 0000  ..rb...c........
-00001240: 0000 0000 0100 0000 0300 0000 5300 0000  ............S...
-00001250: 730e 0000 0074 006a 016a 02a0 037c 00a1  s....t.j.j...|..
-00001260: 0153 0072 5b00 0000 725c 0000 0072 5f00  .S.r[...r\...r_.
-00001270: 0000 723d 0000 0072 3d00 0000 723e 0000  ..r=...r=...r>..
-00001280: 0072 6100 0000 c000 0000 7262 0000 0063  .ra.......rb...c
-00001290: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000012a0: 0300 0000 5300 0000 730e 0000 0074 006a  ....S...s....t.j
-000012b0: 016a 02a0 037c 00a1 0153 0072 5b00 0000  .j...|...S.r[...
-000012c0: a904 720b 0000 0072 2100 0000 da0e 5065  ..r....r!.....Pe
-000012d0: 7270 5061 7261 6d65 7465 7273 725e 0000  rpParametersr^..
-000012e0: 0072 5f00 0000 723d 0000 0072 3d00 0000  .r_...r=...r=...
-000012f0: 723e 0000 0072 6100 0000 d000 0000 7262  r>...ra.......rb
-00001300: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001310: 0100 0000 0300 0000 5300 0000 730e 0000  ........S...s...
-00001320: 0074 006a 016a 02a0 037c 00a1 0153 0072  .t.j.j...|...S.r
-00001330: 5b00 0000 7263 0000 0072 5f00 0000 723d  [...rc...r_...r=
-00001340: 0000 0072 3d00 0000 723e 0000 0072 6100  ...r=...r>...ra.
-00001350: 0000 d600 0000 7262 0000 0063 0100 0000  ......rb...c....
-00001360: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00001370: 5300 0000 730e 0000 0074 006a 016a 02a0  S...s....t.j.j..
-00001380: 037c 00a1 0153 0072 5b00 0000 a904 720b  .|...S.r[.....r.
-00001390: 0000 0072 2300 0000 da10 4d61 7267 696e  ...r#.....Margin
-000013a0: 5061 7261 6d65 7465 7273 725e 0000 0072  Parametersr^...r
-000013b0: 5f00 0000 723d 0000 0072 3d00 0000 723e  _...r=...r=...r>
-000013c0: 0000 0072 6100 0000 dc00 0000 7262 0000  ...ra.......rb..
-000013d0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-000013e0: 0000 0300 0000 5300 0000 730e 0000 0074  ......S...s....t
-000013f0: 006a 016a 02a0 037c 00a1 0153 0072 5b00  .j.j...|...S.r[.
-00001400: 0000 7265 0000 0072 5f00 0000 723d 0000  ..re...r_...r=..
-00001410: 0072 3d00 0000 723e 0000 0072 6100 0000  .r=...r>...ra...
-00001420: e200 0000 7262 0000 0063 0100 0000 0000  ....rb...c......
-00001430: 0000 0000 0000 0100 0000 0300 0000 5300  ..............S.
-00001440: 0000 730e 0000 0074 006a 016a 02a0 037c  ..s....t.j.j...|
-00001450: 00a1 0153 0072 5b00 0000 a904 720b 0000  ...S.r[.....r...
-00001460: 0072 3a00 0000 da07 5072 6f64 7563 7472  .r:.....Productr
-00001470: 5e00 0000 725f 0000 0072 3d00 0000 723d  ^...r_...r=...r=
-00001480: 0000 0072 3e00 0000 7261 0000 00e6 0000  ...r>...ra......
-00001490: 0072 6200 0000 6301 0000 0000 0000 0000  .rb...c.........
-000014a0: 0000 0001 0000 0003 0000 0053 0000 0073  ...........S...s
-000014b0: 0e00 0000 7400 6a01 6a02 a003 7c00 a101  ....t.j.j...|...
-000014c0: 5300 725b 0000 0072 6700 0000 725f 0000  S.r[...rg...r_..
-000014d0: 0072 3d00 0000 723d 0000 0072 3e00 0000  .r=...r=...r>...
-000014e0: 7261 0000 00e9 0000 0072 6200 0000 a921  ra.......rb....!
-000014f0: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00001500: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
-00001510: 0000 0072 1500 0000 7216 0000 0072 1700  ...r....r....r..
-00001520: 0000 7218 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00001530: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00001540: 721e 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
-00001550: 2100 0000 7222 0000 0072 2300 0000 7224  !...r"...r#...r$
-00001560: 0000 0072 2500 0000 7226 0000 0072 2700  ...r%...r&...r'.
-00001570: 0000 7228 0000 0072 2900 0000 722a 0000  ..r(...r)...r*..
-00001580: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
-00001590: 722e 0000 0029 2972 0400 0000 7240 0000  r....))r....r@..
-000015a0: 0072 0500 0000 723f 0000 0072 4300 0000  .r....r?...rC...
-000015b0: da05 7061 7273 6572 0e00 0000 720f 0000  ..parser....r...
-000015c0: 0072 1000 0000 7211 0000 0072 1200 0000  .r....r....r....
-000015d0: 7234 0000 00da 036d 6170 7213 0000 0072  r4.....mapr....r
-000015e0: 1400 0000 7215 0000 0072 1600 0000 7217  ....r....r....r.
-000015f0: 0000 0072 1800 0000 7219 0000 0072 1a00  ...r....r....r..
-00001600: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-00001610: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
-00001620: 7221 0000 0072 2200 0000 7223 0000 0072  r!...r"...r#...r
-00001630: 2400 0000 7225 0000 0072 2600 0000 7227  $...r%...r&...r'
-00001640: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
-00001650: 0000 722b 0000 0072 2c00 0000 722d 0000  ..r+...r,...r-..
-00001660: 0072 2e00 0000 2903 7250 0000 0072 4e00  .r....).rP...rN.
-00001670: 0000 da03 6465 6372 3d00 0000 723d 0000  ....decr=...r=..
-00001680: 0072 3e00 0000 724f 0000 00a1 0000 0073  .r>...rO.......s
-00001690: a600 0000 0002 1201 0801 1401 0201 0401  ................
-000016a0: 0401 0401 0401 0401 0201 0201 0601 04fe  ................
-000016b0: 02ff 0206 0201 0201 0601 04fe 02ff 0206  ................
-000016c0: 0201 0201 0601 04fe 02ff 0206 0201 0201  ................
-000016d0: 0601 04fe 02ff 0206 0401 0401 0401 0401  ................
-000016e0: 0401 0401 0401 0401 0401 0401 0201 0201  ................
-000016f0: 0601 04fe 02ff 0206 0201 0201 0601 04fe  ................
-00001700: 02ff 0206 0201 0201 0601 04fe 02ff 0206  ................
-00001710: 0201 0201 0601 04fe 02ff 0206 1201 0201  ................
-00001720: 0201 0601 04fe 02ff 0206 0401 0401 0401  ................
-00001730: 0401 0401 0401 0401 04b2 7a0e 5072 6963  ..........z.Pric
-00001740: 696e 672e 6465 636f 6465 2901 7248 0000  ing.decode).rH..
-00001750: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00001760: 0000 2200 0000 4300 0000 73a2 0100 007c  .."...C...s....|
-00001770: 006a 007c 006a 017c 006a 027c 006a 037c  .j.|.j.|.j.|.j.|
-00001780: 006a 0474 0574 0664 0164 0284 007c 006a  .j.t.t.d.d...|.j
-00001790: 0783 0283 0174 0574 0664 0364 0284 007c  .....t.t.d.d...|
-000017a0: 006a 0883 0283 0174 0574 0664 0464 0284  .j.....t.t.d.d..
-000017b0: 007c 006a 0983 0283 0174 0574 0664 0564  .|.j.....t.t.d.d
-000017c0: 0284 007c 006a 0a83 0283 017c 006a 0b7c  ...|.j.....|.j.|
-000017d0: 006a 0c74 0574 0664 0664 0284 007c 006a  .j.t.t.d.d...|.j
-000017e0: 0d83 0283 0174 0574 0664 0764 0284 007c  .....t.t.d.d...|
-000017f0: 006a 0e83 0283 0174 0574 0664 0864 0284  .j.....t.t.d.d..
-00001800: 007c 006a 0f83 0283 0174 0574 0664 0964  .|.j.....t.t.d.d
-00001810: 0284 007c 006a 1083 0283 0174 0574 0664  ...|.j.....t.t.d
-00001820: 0a64 0284 007c 006a 1183 0283 0174 0574  .d...|.j.....t.t
-00001830: 0664 0b64 0284 007c 006a 1283 0283 0174  .d.d...|.j.....t
-00001840: 0574 0664 0c64 0284 007c 006a 1383 0283  .t.d.d...|.j....
-00001850: 0174 0574 0664 0d64 0284 007c 006a 1483  .t.t.d.d...|.j..
-00001860: 0283 0174 0574 0664 0e64 0284 007c 006a  ...t.t.d.d...|.j
-00001870: 1583 0283 0174 0574 0664 0f64 0284 007c  .....t.t.d.d...|
-00001880: 006a 1683 0283 0174 0574 0664 1064 0284  .j.....t.t.d.d..
-00001890: 007c 006a 1783 0283 0174 0574 0664 1164  .|.j.....t.t.d.d
-000018a0: 0284 007c 006a 1883 0283 0174 0574 0664  ...|.j.....t.t.d
-000018b0: 1264 0284 007c 006a 1983 0283 0174 0574  .d...|.j.....t.t
-000018c0: 0664 1364 0284 007c 006a 1a83 0283 0174  .d.d...|.j.....t
-000018d0: 0574 0664 1464 0284 007c 006a 1b83 0283  .t.d.d...|.j....
-000018e0: 0174 0574 0664 1564 0284 007c 006a 1c83  .t.t.d.d...|.j..
-000018f0: 0283 017c 006a 1d7c 006a 1e7c 006a 1f7c  ...|.j.|.j.|.j.|
-00001900: 006a 207c 006a 217c 006a 2264 169c 2153  .j |.j!|.j"d..!S
-00001910: 0029 174e 6301 0000 0000 0000 0000 0000  .).Nc...........
-00001920: 0001 0000 0002 0000 0053 0000 0073 0800  .........S...s..
-00001930: 0000 7c00 a000 a100 5300 725b 0000 00a9  ..|.....S.r[....
-00001940: 01da 0774 6f5f 6a73 6f6e 725f 0000 0072  ...to_jsonr_...r
-00001950: 3d00 0000 723d 0000 0072 3e00 0000 7261  =...r=...r>...ra
-00001960: 0000 00fe 0000 0072 6200 0000 7a21 5072  .......rb...z!Pr
-00001970: 6963 696e 672e 746f 5f6a 736f 6e2e 3c6c  icing.to_json.<l
-00001980: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e63  ocals>.<lambda>c
-00001990: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000019a0: 0200 0000 5300 0000 7308 0000 007c 00a0  ....S...s....|..
-000019b0: 00a1 0053 0072 5b00 0000 726d 0000 0072  ...S.r[...rm...r
-000019c0: 5f00 0000 723d 0000 0072 3d00 0000 723e  _...r=...r=...r>
-000019d0: 0000 0072 6100 0000 ff00 0000 7262 0000  ...ra.......rb..
-000019e0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-000019f0: 0000 0200 0000 5300 0000 7308 0000 007c  ......S...s....|
-00001a00: 00a0 00a1 0053 0072 5b00 0000 726d 0000  .....S.r[...rm..
-00001a10: 0072 5f00 0000 723d 0000 0072 3d00 0000  .r_...r=...r=...
-00001a20: 723e 0000 0072 6100 0000 0001 0000 7262  r>...ra.......rb
-00001a30: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001a40: 0100 0000 0200 0000 5300 0000 7308 0000  ........S...s...
-00001a50: 007c 00a0 00a1 0053 0072 5b00 0000 726d  .|.....S.r[...rm
-00001a60: 0000 0072 5f00 0000 723d 0000 0072 3d00  ...r_...r=...r=.
-00001a70: 0000 723e 0000 0072 6100 0000 0101 0000  ..r>...ra.......
-00001a80: 7262 0000 0063 0100 0000 0000 0000 0000  rb...c..........
-00001a90: 0000 0100 0000 0200 0000 5300 0000 7308  ..........S...s.
-00001aa0: 0000 0074 007c 0083 0153 0072 5b00 0000  ...t.|...S.r[...
-00001ab0: a901 7237 0000 0072 5f00 0000 723d 0000  ..r7...r_...r=..
-00001ac0: 0072 3d00 0000 723e 0000 0072 6100 0000  .r=...r>...ra...
-00001ad0: 0401 0000 7262 0000 0063 0100 0000 0000  ....rb...c......
-00001ae0: 0000 0000 0000 0100 0000 0200 0000 5300  ..............S.
-00001af0: 0000 7308 0000 0074 007c 0083 0153 0072  ..s....t.|...S.r
-00001b00: 5b00 0000 726f 0000 0072 5f00 0000 723d  [...ro...r_...r=
-00001b10: 0000 0072 3d00 0000 723e 0000 0072 6100  ...r=...r>...ra.
-00001b20: 0000 0501 0000 7262 0000 0063 0100 0000  ......rb...c....
-00001b30: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00001b40: 5300 0000 7308 0000 0074 007c 0083 0153  S...s....t.|...S
-00001b50: 0072 5b00 0000 726f 0000 0072 5f00 0000  .r[...ro...r_...
-00001b60: 723d 0000 0072 3d00 0000 723e 0000 0072  r=...r=...r>...r
-00001b70: 6100 0000 0601 0000 7262 0000 0063 0100  a.......rb...c..
-00001b80: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00001b90: 0000 5300 0000 7308 0000 0074 007c 0083  ..S...s....t.|..
-00001ba0: 0153 0072 5b00 0000 726f 0000 0072 5f00  .S.r[...ro...r_.
-00001bb0: 0000 723d 0000 0072 3d00 0000 723e 0000  ..r=...r=...r>..
-00001bc0: 0072 6100 0000 0701 0000 7262 0000 0063  .ra.......rb...c
-00001bd0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00001be0: 0200 0000 5300 0000 7308 0000 0074 007c  ....S...s....t.|
-00001bf0: 0083 0153 0072 5b00 0000 726f 0000 0072  ...S.r[...ro...r
-00001c00: 5f00 0000 723d 0000 0072 3d00 0000 723e  _...r=...r=...r>
-00001c10: 0000 0072 6100 0000 0801 0000 7262 0000  ...ra.......rb..
-00001c20: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00001c30: 0000 0200 0000 5300 0000 7308 0000 0074  ......S...s....t
-00001c40: 007c 0083 0153 0072 5b00 0000 726f 0000  .|...S.r[...ro..
-00001c50: 0072 5f00 0000 723d 0000 0072 3d00 0000  .r_...r=...r=...
-00001c60: 723e 0000 0072 6100 0000 0901 0000 7262  r>...ra.......rb
-00001c70: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001c80: 0100 0000 0200 0000 5300 0000 7308 0000  ........S...s...
-00001c90: 0074 007c 0083 0153 0072 5b00 0000 726f  .t.|...S.r[...ro
-00001ca0: 0000 0072 5f00 0000 723d 0000 0072 3d00  ...r_...r=...r=.
-00001cb0: 0000 723e 0000 0072 6100 0000 0a01 0000  ..r>...ra.......
-00001cc0: 7262 0000 0063 0100 0000 0000 0000 0000  rb...c..........
-00001cd0: 0000 0100 0000 0200 0000 5300 0000 7308  ..........S...s.
-00001ce0: 0000 0074 007c 0083 0153 0072 5b00 0000  ...t.|...S.r[...
-00001cf0: 726f 0000 0072 5f00 0000 723d 0000 0072  ro...r_...r=...r
-00001d00: 3d00 0000 723e 0000 0072 6100 0000 0b01  =...r>...ra.....
-00001d10: 0000 7262 0000 0063 0100 0000 0000 0000  ..rb...c........
-00001d20: 0000 0000 0100 0000 0200 0000 5300 0000  ............S...
-00001d30: 7308 0000 007c 00a0 00a1 0053 0072 5b00  s....|.....S.r[.
-00001d40: 0000 726d 0000 0072 5f00 0000 723d 0000  ..rm...r_...r=..
-00001d50: 0072 3d00 0000 723e 0000 0072 6100 0000  .r=...r>...ra...
-00001d60: 0c01 0000 7262 0000 0063 0100 0000 0000  ....rb...c......
-00001d70: 0000 0000 0000 0100 0000 0200 0000 5300  ..............S.
-00001d80: 0000 7308 0000 007c 00a0 00a1 0053 0072  ..s....|.....S.r
-00001d90: 5b00 0000 726d 0000 0072 5f00 0000 723d  [...rm...r_...r=
-00001da0: 0000 0072 3d00 0000 723e 0000 0072 6100  ...r=...r>...ra.
-00001db0: 0000 0d01 0000 7262 0000 0063 0100 0000  ......rb...c....
-00001dc0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00001dd0: 5300 0000 7308 0000 007c 00a0 00a1 0053  S...s....|.....S
-00001de0: 0072 5b00 0000 726d 0000 0072 5f00 0000  .r[...rm...r_...
-00001df0: 723d 0000 0072 3d00 0000 723e 0000 0072  r=...r=...r>...r
-00001e00: 6100 0000 0e01 0000 7262 0000 0063 0100  a.......rb...c..
-00001e10: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00001e20: 0000 5300 0000 7308 0000 007c 00a0 00a1  ..S...s....|....
-00001e30: 0053 0072 5b00 0000 726d 0000 0072 5f00  .S.r[...rm...r_.
-00001e40: 0000 723d 0000 0072 3d00 0000 723e 0000  ..r=...r=...r>..
-00001e50: 0072 6100 0000 0f01 0000 7262 0000 0063  .ra.......rb...c
-00001e60: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00001e70: 0200 0000 5300 0000 7308 0000 007c 00a0  ....S...s....|..
-00001e80: 00a1 0053 0072 5b00 0000 726d 0000 0072  ...S.r[...rm...r
-00001e90: 5f00 0000 723d 0000 0072 3d00 0000 723e  _...r=...r=...r>
-00001ea0: 0000 0072 6100 0000 1001 0000 7262 0000  ...ra.......rb..
-00001eb0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00001ec0: 0000 0200 0000 5300 0000 7308 0000 007c  ......S...s....|
-00001ed0: 00a0 00a1 0053 0072 5b00 0000 726d 0000  .....S.r[...rm..
-00001ee0: 0072 5f00 0000 723d 0000 0072 3d00 0000  .r_...r=...r=...
-00001ef0: 723e 0000 0072 6100 0000 1101 0000 7262  r>...ra.......rb
-00001f00: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001f10: 0100 0000 0200 0000 5300 0000 7308 0000  ........S...s...
-00001f20: 0074 007c 0083 0153 0072 5b00 0000 726f  .t.|...S.r[...ro
-00001f30: 0000 0072 5f00 0000 723d 0000 0072 3d00  ...r_...r=...r=.
-00001f40: 0000 723e 0000 0072 6100 0000 1201 0000  ..r>...ra.......
-00001f50: 7262 0000 0063 0100 0000 0000 0000 0000  rb...c..........
-00001f60: 0000 0100 0000 0200 0000 5300 0000 7308  ..........S...s.
-00001f70: 0000 0074 007c 0083 0153 0072 5b00 0000  ...t.|...S.r[...
-00001f80: 726f 0000 0072 5f00 0000 723d 0000 0072  ro...r_...r=...r
-00001f90: 3d00 0000 723e 0000 0072 6100 0000 1301  =...r>...ra.....
-00001fa0: 0000 7262 0000 0072 6900 0000 2923 720e  ..rb...ri...)#r.
-00001fb0: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
-00001fc0: 0000 7212 0000 0072 3400 0000 726b 0000  ..r....r4...rk..
-00001fd0: 0072 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
-00001fe0: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
-00001ff0: 1900 0000 721a 0000 0072 1b00 0000 721c  ....r....r....r.
-00002000: 0000 0072 1d00 0000 721e 0000 0072 1f00  ...r....r....r..
-00002010: 0000 7220 0000 0072 2100 0000 7222 0000  ..r ...r!...r"..
-00002020: 0072 2300 0000 7224 0000 0072 2500 0000  .r#...r$...r%...
-00002030: 7226 0000 0072 2700 0000 7228 0000 0072  r&...r'...r(...r
-00002040: 2900 0000 722a 0000 0072 2b00 0000 722c  )...r*...r+...r,
-00002050: 0000 0072 2d00 0000 722e 0000 0029 01da  ...r-...r....)..
-00002060: 0473 656c 6672 3d00 0000 723d 0000 0072  .selfr=...r=...r
-00002070: 3e00 0000 726e 0000 00f7 0000 0073 4400  >...rn.......sD.
-00002080: 0000 0002 0401 0401 0401 0401 0401 1201  ................
-00002090: 1201 1201 1201 0401 0401 1201 1201 1201  ................
-000020a0: 1201 1201 1201 1201 1201 1201 1201 1201  ................
-000020b0: 1201 1201 1201 1201 1201 0401 0401 0401  ................
-000020c0: 0401 0401 04df 7a0f 5072 6963 696e 672e  ......z.Pricing.
-000020d0: 746f 5f6a 736f 6e29 02da 036f 626a 7248  to_json)...objrH
-000020e0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-000020f0: 0200 0000 2300 0000 4300 0000 73e6 0100  ....#...C...s...
-00002100: 007c 007c 0164 0119 007c 0164 0219 007c  .|.|.d...|.d...|
-00002110: 0164 0319 007c 0164 0419 007c 0164 0519  .d...|.d...|.d..
-00002120: 0074 0074 0164 0664 0784 007c 0164 0819  .t.t.d.d...|.d..
-00002130: 0083 0283 0174 0074 0164 0964 0784 007c  .....t.t.d.d...|
-00002140: 0164 0a19 0083 0283 0174 0074 0164 0b64  .d.......t.t.d.d
-00002150: 0784 007c 0164 0c19 0083 0283 0174 0074  ...|.d.......t.t
-00002160: 0164 0d64 0784 007c 0164 0e19 0083 0283  .d.d...|.d......
-00002170: 017c 0164 0f19 007c 0164 1019 0074 0074  .|.d...|.d...t.t
-00002180: 0164 1164 0784 007c 0164 1219 0083 0283  .d.d...|.d......
-00002190: 0174 0074 0164 1364 0784 007c 0164 1419  .t.t.d.d...|.d..
-000021a0: 0083 0283 0174 0074 0164 1564 0784 007c  .....t.t.d.d...|
-000021b0: 0164 1619 0083 0283 0174 0074 0164 1764  .d.......t.t.d.d
-000021c0: 0784 007c 0164 1819 0083 0283 0174 0074  ...|.d.......t.t
-000021d0: 0164 1964 0784 007c 0164 1a19 0083 0283  .d.d...|.d......
-000021e0: 0174 0074 0164 1b64 0784 007c 0164 1c19  .t.t.d.d...|.d..
-000021f0: 0083 0283 0174 0074 0164 1d64 0784 007c  .....t.t.d.d...|
-00002200: 0164 1e19 0083 0283 0174 0074 0164 1f64  .d.......t.t.d.d
-00002210: 0784 007c 0164 2019 0083 0283 0174 0074  ...|.d ......t.t
-00002220: 0164 2164 0784 007c 0164 2219 0083 0283  .d!d...|.d".....
-00002230: 0174 0074 0164 2364 0784 007c 0164 2419  .t.t.d#d...|.d$.
-00002240: 0083 0283 0174 0074 0164 2564 0784 007c  .....t.t.d%d...|
-00002250: 0164 2619 0083 0283 0174 0074 0164 2764  .d&......t.t.d'd
-00002260: 0784 007c 0164 2819 0083 0283 0174 0074  ...|.d(......t.t
-00002270: 0164 2964 0784 007c 0164 2a19 0083 0283  .d)d...|.d*.....
-00002280: 0174 0074 0164 2b64 0784 007c 0164 2c19  .t.t.d+d...|.d,.
-00002290: 0083 0283 0174 0074 0164 2d64 0784 007c  .....t.t.d-d...|
-000022a0: 0164 2e19 0083 0283 0174 0074 0164 2f64  .d.......t.t.d/d
-000022b0: 0784 007c 0164 3019 0083 0283 017c 0164  ...|.d0......|.d
-000022c0: 3119 007c 0164 3219 007c 0164 3319 007c  1..|.d2..|.d3..|
-000022d0: 0164 3419 007c 0164 3519 007c 0164 3619  .d4..|.d5..|.d6.
-000022e0: 0064 378d 2153 0029 384e 720e 0000 0072  .d7.!S.)8Nr....r
-000022f0: 0f00 0000 7210 0000 0072 1100 0000 7212  ....r....r....r.
-00002300: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00002310: 0100 0000 0300 0000 5300 0000 730e 0000  ........S...s...
-00002320: 0074 006a 016a 02a0 037c 00a1 0153 0072  .t.j.j...|...S.r
-00002330: 5b00 0000 a904 720b 0000 0072 3500 0000  [.....r....r5...
-00002340: 725d 0000 00da 0966 726f 6d5f 6a73 6f6e  r].....from_json
-00002350: 725f 0000 0072 3d00 0000 723d 0000 0072  r_...r=...r=...r
-00002360: 3e00 0000 7261 0000 0026 0100 0072 6200  >...ra...&...rb.
-00002370: 0000 7a23 5072 6963 696e 672e 6672 6f6d  ..z#Pricing.from
-00002380: 5f6a 736f 6e2e 3c6c 6f63 616c 733e 2e3c  _json.<locals>.<
-00002390: 6c61 6d62 6461 3e72 1300 0000 6301 0000  lambda>r....c...
-000023a0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-000023b0: 0053 0000 0073 0e00 0000 7400 6a01 6a02  .S...s....t.j.j.
-000023c0: a003 7c00 a101 5300 725b 0000 0072 7200  ..|...S.r[...rr.
-000023d0: 0000 725f 0000 0072 3d00 0000 723d 0000  ..r_...r=...r=..
-000023e0: 0072 3e00 0000 7261 0000 002c 0100 0072  .r>...ra...,...r
-000023f0: 6200 0000 7214 0000 0063 0100 0000 0000  b...r....c......
-00002400: 0000 0000 0000 0100 0000 0300 0000 5300  ..............S.
-00002410: 0000 730e 0000 0074 006a 016a 02a0 037c  ..s....t.j.j...|
-00002420: 00a1 0153 0072 5b00 0000 7272 0000 0072  ...S.r[...rr...r
-00002430: 5f00 0000 723d 0000 0072 3d00 0000 723e  _...r=...r=...r>
-00002440: 0000 0072 6100 0000 3201 0000 7262 0000  ...ra...2...rb..
-00002450: 0072 1500 0000 6301 0000 0000 0000 0000  .r....c.........
-00002460: 0000 0001 0000 0003 0000 0053 0000 0073  ...........S...s
-00002470: 0e00 0000 7400 6a01 6a02 a003 7c00 a101  ....t.j.j...|...
-00002480: 5300 725b 0000 0072 7200 0000 725f 0000  S.r[...rr...r_..
-00002490: 0072 3d00 0000 723d 0000 0072 3e00 0000  .r=...r=...r>...
-000024a0: 7261 0000 0038 0100 0072 6200 0000 7216  ra...8...rb...r.
-000024b0: 0000 0072 1700 0000 7218 0000 0063 0100  ...r....r....c..
-000024c0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-000024d0: 0000 5300 0000 730a 0000 0074 00a0 017c  ..S...s....t...|
-000024e0: 00a1 0153 0072 5b00 0000 a902 7209 0000  ...S.r[.....r...
-000024f0: 00da 0b66 726f 6d5f 7374 7269 6e67 725f  ...from_stringr_
-00002500: 0000 0072 3d00 0000 723d 0000 0072 3e00  ...r=...r=...r>.
-00002510: 0000 7261 0000 003e 0100 0072 6200 0000  ..ra...>...rb...
-00002520: 7219 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00002530: 0000 0100 0000 0300 0000 5300 0000 730a  ..........S...s.
-00002540: 0000 0074 00a0 017c 00a1 0153 0072 5b00  ...t...|...S.r[.
-00002550: 0000 7274 0000 0072 5f00 0000 723d 0000  ..rt...r_...r=..
-00002560: 0072 3d00 0000 723e 0000 0072 6100 0000  .r=...r>...ra...
-00002570: 3f01 0000 7262 0000 0072 1a00 0000 6301  ?...rb...r....c.
-00002580: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00002590: 0000 0053 0000 0073 0a00 0000 7400 a001  ...S...s....t...
-000025a0: 7c00 a101 5300 725b 0000 0072 7400 0000  |...S.r[...rt...
-000025b0: 725f 0000 0072 3d00 0000 723d 0000 0072  r_...r=...r=...r
-000025c0: 3e00 0000 7261 0000 0040 0100 0072 6200  >...ra...@...rb.
-000025d0: 0000 721b 0000 0063 0100 0000 0000 0000  ..r....c........
-000025e0: 0000 0000 0100 0000 0300 0000 5300 0000  ............S...
-000025f0: 730a 0000 0074 00a0 017c 00a1 0153 0072  s....t...|...S.r
-00002600: 5b00 0000 7274 0000 0072 5f00 0000 723d  [...rt...r_...r=
-00002610: 0000 0072 3d00 0000 723e 0000 0072 6100  ...r=...r>...ra.
-00002620: 0000 4301 0000 7262 0000 0072 1c00 0000  ..C...rb...r....
-00002630: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00002640: 0003 0000 0053 0000 0073 0a00 0000 7400  .....S...s....t.
-00002650: a001 7c00 a101 5300 725b 0000 0072 7400  ..|...S.r[...rt.
-00002660: 0000 725f 0000 0072 3d00 0000 723d 0000  ..r_...r=...r=..
-00002670: 0072 3e00 0000 7261 0000 0047 0100 0072  .r>...ra...G...r
-00002680: 6200 0000 721d 0000 0063 0100 0000 0000  b...r....c......
-00002690: 0000 0000 0000 0100 0000 0300 0000 5300  ..............S.
-000026a0: 0000 730a 0000 0074 00a0 017c 00a1 0153  ..s....t...|...S
-000026b0: 0072 5b00 0000 7274 0000 0072 5f00 0000  .r[...rt...r_...
-000026c0: 723d 0000 0072 3d00 0000 723e 0000 0072  r=...r=...r>...r
-000026d0: 6100 0000 4801 0000 7262 0000 0072 1e00  a...H...rb...r..
-000026e0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-000026f0: 0000 0003 0000 0053 0000 0073 0a00 0000  .......S...s....
-00002700: 7400 a001 7c00 a101 5300 725b 0000 0072  t...|...S.r[...r
-00002710: 7400 0000 725f 0000 0072 3d00 0000 723d  t...r_...r=...r=
-00002720: 0000 0072 3e00 0000 7261 0000 0049 0100  ...r>...ra...I..
-00002730: 0072 6200 0000 721f 0000 0063 0100 0000  .rb...r....c....
-00002740: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00002750: 5300 0000 730a 0000 0074 00a0 017c 00a1  S...s....t...|..
-00002760: 0153 0072 5b00 0000 7274 0000 0072 5f00  .S.r[...rt...r_.
-00002770: 0000 723d 0000 0072 3d00 0000 723e 0000  ..r=...r=...r>..
-00002780: 0072 6100 0000 4c01 0000 7262 0000 0072  .ra...L...rb...r
-00002790: 2000 0000 6301 0000 0000 0000 0000 0000   ...c...........
-000027a0: 0001 0000 0003 0000 0053 0000 0073 0e00  .........S...s..
-000027b0: 0000 7400 6a01 6a02 a003 7c00 a101 5300  ..t.j.j...|...S.
-000027c0: 725b 0000 00a9 0472 0b00 0000 7221 0000  r[.....r....r!..
-000027d0: 0072 6400 0000 7273 0000 0072 5f00 0000  .rd...rs...r_...
-000027e0: 723d 0000 0072 3d00 0000 723e 0000 0072  r=...r=...r>...r
-000027f0: 6100 0000 5201 0000 7262 0000 0072 2100  a...R...rb...r!.
-00002800: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00002810: 0000 0003 0000 0053 0000 0073 0e00 0000  .......S...s....
-00002820: 7400 6a01 6a02 a003 7c00 a101 5300 725b  t.j.j...|...S.r[
-00002830: 0000 0072 7600 0000 725f 0000 0072 3d00  ...rv...r_...r=.
-00002840: 0000 723d 0000 0072 3e00 0000 7261 0000  ..r=...r>...ra..
-00002850: 0058 0100 0072 6200 0000 7222 0000 0063  .X...rb...r"...c
-00002860: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00002870: 0300 0000 5300 0000 730e 0000 0074 006a  ....S...s....t.j
-00002880: 016a 02a0 037c 00a1 0153 0072 5b00 0000  .j...|...S.r[...
-00002890: a904 720b 0000 0072 2300 0000 7266 0000  ..r....r#...rf..
-000028a0: 0072 7300 0000 725f 0000 0072 3d00 0000  .rs...r_...r=...
-000028b0: 723d 0000 0072 3e00 0000 7261 0000 005e  r=...r>...ra...^
-000028c0: 0100 0072 6200 0000 7223 0000 0063 0100  ...rb...r#...c..
-000028d0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-000028e0: 0000 5300 0000 730e 0000 0074 006a 016a  ..S...s....t.j.j
-000028f0: 02a0 037c 00a1 0153 0072 5b00 0000 7277  ...|...S.r[...rw
-00002900: 0000 0072 5f00 0000 723d 0000 0072 3d00  ...r_...r=...r=.
-00002910: 0000 723e 0000 0072 6100 0000 6401 0000  ..r>...ra...d...
-00002920: 7262 0000 0072 2400 0000 6301 0000 0000  rb...r$...c.....
-00002930: 0000 0000 0000 0001 0000 0003 0000 0053  ...............S
-00002940: 0000 0073 0e00 0000 7400 6a01 6a02 a003  ...s....t.j.j...
-00002950: 7c00 a101 5300 725b 0000 00a9 0472 0b00  |...S.r[.....r..
-00002960: 0000 723a 0000 0072 6800 0000 7273 0000  ..r:...rh...rs..
-00002970: 0072 5f00 0000 723d 0000 0072 3d00 0000  .r_...r=...r=...
-00002980: 723e 0000 0072 6100 0000 6801 0000 7262  r>...ra...h...rb
-00002990: 0000 0072 2500 0000 6301 0000 0000 0000  ...r%...c.......
-000029a0: 0000 0000 0001 0000 0003 0000 0053 0000  .............S..
-000029b0: 0073 0e00 0000 7400 6a01 6a02 a003 7c00  .s....t.j.j...|.
-000029c0: a101 5300 725b 0000 0072 7800 0000 725f  ..S.r[...rx...r_
-000029d0: 0000 0072 3d00 0000 723d 0000 0072 3e00  ...r=...r=...r>.
-000029e0: 0000 7261 0000 006b 0100 0072 6200 0000  ..ra...k...rb...
-000029f0: 7226 0000 0063 0100 0000 0000 0000 0000  r&...c..........
-00002a00: 0000 0100 0000 0300 0000 5300 0000 730a  ..........S...s.
-00002a10: 0000 0074 00a0 017c 00a1 0153 0072 5b00  ...t...|...S.r[.
-00002a20: 0000 7274 0000 0072 5f00 0000 723d 0000  ..rt...r_...r=..
-00002a30: 0072 3d00 0000 723e 0000 0072 6100 0000  .r=...r>...ra...
-00002a40: 6f01 0000 7262 0000 0072 2700 0000 6301  o...rb...r'...c.
-00002a50: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00002a60: 0000 0053 0000 0073 0a00 0000 7400 a001  ...S...s....t...
-00002a70: 7c00 a101 5300 725b 0000 0072 7400 0000  |...S.r[...rt...
-00002a80: 725f 0000 0072 3d00 0000 723d 0000 0072  r_...r=...r=...r
-00002a90: 3e00 0000 7261 0000 0072 0100 0072 6200  >...ra...r...rb.
-00002aa0: 0000 7228 0000 0072 2900 0000 722a 0000  ..r(...r)...r*..
-00002ab0: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
-00002ac0: 722e 0000 0072 6900 0000 2902 7234 0000  r....ri...).r4..
-00002ad0: 0072 6b00 0000 2902 7250 0000 0072 7100  .rk...).rP...rq.
-00002ae0: 0000 723d 0000 0072 3d00 0000 723e 0000  ..r=...r=...r>..
-00002af0: 0072 7300 0000 1c01 0000 73be 0000 0000  .rs.......s.....
-00002b00: 0202 0106 0106 0106 0106 0106 0102 0102  ................
-00002b10: 0106 0106 fe02 ff02 0602 0102 0106 0106  ................
-00002b20: fe02 ff02 0602 0102 0106 0106 fe02 ff02  ................
-00002b30: 0602 0102 0106 0106 fe02 ff02 0606 0106  ................
-00002b40: 0114 0114 0114 0102 0102 0106 0106 fe02  ................
-00002b50: ff02 0614 0114 0114 0102 0102 0106 0106  ................
-00002b60: fe02 ff02 0602 0102 0106 0106 fe02 ff02  ................
-00002b70: 0602 0102 0106 0106 fe02 ff02 0602 0102  ................
-00002b80: 0106 0106 fe02 ff02 0602 0102 0106 0106  ................
-00002b90: fe02 ff02 0614 0102 0102 0106 0106 fe02  ................
+000006f0: 7473 2f7a 6574 612f 7a65 7461 6d61 726b  ts/zeta/zetamark
+00000700: 6574 732d 7079 2f7a 6574 616d 6172 6b65  ets-py/zetamarke
+00000710: 7473 5f70 792f 7a65 7461 5f63 6c69 656e  ts_py/zeta_clien
+00000720: 742f 6163 636f 756e 7473 2f70 7269 6369  t/accounts/prici
+00000730: 6e67 2e70 7972 0d00 0000 1100 0000 7342  ng.pyr........sB
+00000740: 0000 000a 0108 010c 010c 010c 010c 0110  ................
+00000750: 0110 0110 0110 010c 010c 010c 010c 010c  ................
+00000760: 010c 010c 010c 010c 010c 0110 0110 0110  ................
+00000770: 0110 0110 0110 010c 010c 0108 0108 0108  ................
+00000780: 010c 010c 0172 0d00 0000 6300 0000 0000  .....r....c.....
+00000790: 0000 0000 0000 0000 0000 0025 0000 0040  ...........%...@
+000007a0: 0000 0073 fa03 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+000007b0: 5500 6401 5a03 6504 6a05 6506 6402 3c00  U.d.Z.e.j.e.d.<.
+000007c0: 6507 a008 6403 6507 6a09 1b00 6404 6507  e...d.e.j...d.e.
+000007d0: 6a0a 6405 1900 1b00 6406 6507 6a0a 6407  j.d.....d.e.j.d.
+000007e0: 1900 1b00 6408 6507 6a0a 6405 1900 1b00  ....d.e.j.d.....
+000007f0: 6409 6507 6a0a 6407 1900 1b00 640a 650b  d.e.j.d.....d.e.
+00000800: 6a0c 6a0d 6a0e 6405 1900 1b00 640b 650b  j.j.j.d.....d.e.
+00000810: 6a0c 6a0d 6a0e 6407 1900 1b00 640c 650b  j.j.j.d.....d.e.
+00000820: 6a0c 6a0d 6a0e 6405 1900 1b00 640d 650b  j.j.j.d.....d.e.
+00000830: 6a0c 6a0d 6a0e 6407 1900 1b00 640e 6507  j.j.j.d.....d.e.
+00000840: 6a0a 6405 1900 1b00 640f 6507 6a0a 6407  j.d.....d.e.j.d.
+00000850: 1900 1b00 6410 650f 6405 1900 1b00 6411  ....d.e.d.....d.
+00000860: 650f 6407 1900 1b00 6412 650f 6405 1900  e.d.....d.e.d...
+00000870: 1b00 6413 650f 6407 1900 1b00 6414 650f  ..d.e.d.....d.e.
+00000880: 6405 1900 1b00 6415 650f 6407 1900 1b00  d.....d.e.d.....
+00000890: 6416 650f 6405 1900 1b00 6417 650f 6407  d.e.d.....d.e.d.
+000008a0: 1900 1b00 6418 650b 6a10 6a11 6a0e 6405  ....d.e.j.j.j.d.
+000008b0: 1900 1b00 6419 650b 6a10 6a11 6a0e 6407  ....d.e.j.j.j.d.
+000008c0: 1900 1b00 641a 650b 6a12 6a13 6a0e 6405  ....d.e.j.j.j.d.
+000008d0: 1900 1b00 641b 650b 6a12 6a13 6a0e 6407  ....d.e.j.j.j.d.
+000008e0: 1900 1b00 641c 650b 6a14 6a15 6a0e 6405  ....d.e.j.j.j.d.
+000008f0: 1900 1b00 641d 650b 6a14 6a15 6a0e 6407  ....d.e.j.j.j.d.
+00000900: 1900 1b00 641e 650f 6405 1900 1b00 641f  ....d.e.d.....d.
+00000910: 650f 6407 1900 1b00 6420 6507 6a0a 1b00  e.d.....d e.j...
+00000920: 6421 6507 6a0a 1b00 6422 6507 6a16 1b00  d!e.j...d"e.j...
+00000930: 6423 6507 6a17 6405 1900 1b00 6424 6507  d#e.j.d.....d$e.
+00000940: 6a17 6407 1900 1b00 6425 6507 6a09 6426  j.d.....d%e.j.d&
+00000950: 1900 1b00 a121 5a0e 6504 6a05 6506 6427  .....!Z.e.j.e.d'
+00000960: 3c00 6518 6506 6403 3c00 6519 6518 1900  <.e.e.d.<.e.e...
+00000970: 6506 6404 3c00 6519 6518 1900 6506 6406  e.d.<.e.e...e.d.
+00000980: 3c00 6519 6518 1900 6506 6408 3c00 6519  <.e.e...e.d.<.e.
+00000990: 6518 1900 6506 6409 3c00 6519 650b 6a0c  e...e.d.<.e.e.j.
+000009a0: 6a0d 1900 6506 640a 3c00 6519 650b 6a0c  j...e.d.<.e.e.j.
+000009b0: 6a0d 1900 6506 640b 3c00 6519 650b 6a0c  j...e.d.<.e.e.j.
+000009c0: 6a0d 1900 6506 640c 3c00 6519 650b 6a0c  j...e.d.<.e.e.j.
+000009d0: 6a0d 1900 6506 640d 3c00 6519 6518 1900  j...e.d.<.e.e...
+000009e0: 6506 640e 3c00 6519 6518 1900 6506 640f  e.d.<.e.e...e.d.
+000009f0: 3c00 6519 651a 1900 6506 6410 3c00 6519  <.e.e...e.d.<.e.
+00000a00: 651a 1900 6506 6411 3c00 6519 651a 1900  e...e.d.<.e.e...
+00000a10: 6506 6412 3c00 6519 651a 1900 6506 6413  e.d.<.e.e...e.d.
+00000a20: 3c00 6519 651a 1900 6506 6414 3c00 6519  <.e.e...e.d.<.e.
+00000a30: 651a 1900 6506 6415 3c00 6519 651a 1900  e...e.d.<.e.e...
+00000a40: 6506 6416 3c00 6519 651a 1900 6506 6417  e.d.<.e.e...e.d.
+00000a50: 3c00 6519 650b 6a10 6a11 1900 6506 6418  <.e.e.j.j...e.d.
+00000a60: 3c00 6519 650b 6a10 6a11 1900 6506 6419  <.e.e.j.j...e.d.
+00000a70: 3c00 6519 650b 6a12 6a13 1900 6506 641a  <.e.e.j.j...e.d.
+00000a80: 3c00 6519 650b 6a12 6a13 1900 6506 641b  <.e.e.j.j...e.d.
+00000a90: 3c00 6519 650b 6a14 6a15 1900 6506 641c  <.e.e.j.j...e.d.
+00000aa0: 3c00 6519 650b 6a14 6a15 1900 6506 641d  <.e.e.j.j...e.d.
+00000ab0: 3c00 6519 651a 1900 6506 641e 3c00 6519  <.e.e...e.d.<.e.
+00000ac0: 651a 1900 6506 641f 3c00 6518 6506 6420  e...e.d.<.e.e.d 
+00000ad0: 3c00 6518 6506 6421 3c00 6518 6506 6422  <.e.e.d!<.e.e.d"
+00000ae0: 3c00 6519 651b 1900 6506 6423 3c00 6519  <.e.e...e.d#<.e.
+00000af0: 651b 1900 6506 6424 3c00 6519 6518 1900  e...e.d$<.e.e...
+00000b00: 6506 6425 3c00 651c 6428 651d 6602 651e  e.d%<.e.d(e.f.e.
+00000b10: 651a 6504 6a1f 6520 1900 651a 6504 6a1f  e.e.j.e ..e.e.j.
+00000b20: 6400 1900 6429 9c05 642a 642b 8405 8301  d...d)..d*d+....
+00000b30: 5a21 651c 6428 651d 6602 651e 6519 651a  Z!e.d(e.f.e.e.e.
+00000b40: 1900 6504 6a1f 6520 1900 651a 6504 6a22  ..e.j.e ..e.e.j"
+00000b50: 6504 6a1f 6400 1900 1900 642c 9c05 642d  e.j.d.....d,..d-
+00000b60: 642e 8405 8301 5a23 651c 6524 6400 642f  d.....Z#e.e$d.d/
+00000b70: 9c02 6430 6431 8404 8301 5a25 6526 6432  ..d0d1....Z%e&d2
+00000b80: 9c01 6433 6434 8404 5a27 651c 6526 6400  ..d3d4..Z'e.e&d.
+00000b90: 6435 9c02 6436 6437 8404 8301 5a28 6428  d5..d6d7....Z(d(
+00000ba0: 5300 2938 da07 5072 6963 696e 6773 0800  S.)8..Pricings..
+00000bb0: 0000 be7b d2b6 8f0b 9888 da0d 6469 7363  ...{........disc
+00000bc0: 7269 6d69 6e61 746f 7272 0e00 0000 720f  riminatorr....r.
+00000bd0: 0000 00e9 0700 0000 7210 0000 00e9 1200  ........r.......
+00000be0: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00000bf0: 0072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000c00: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+00000c10: 1a00 0000 721b 0000 0072 1c00 0000 721d  ....r....r....r.
+00000c20: 0000 0072 1e00 0000 721f 0000 0072 2000  ...r....r....r .
+00000c30: 0000 7221 0000 0072 2200 0000 7223 0000  ..r!...r"...r#..
+00000c40: 0072 2400 0000 7225 0000 0072 2600 0000  .r$...r%...r&...
+00000c50: 7227 0000 0072 2800 0000 7229 0000 0072  r'...r(...r)...r
+00000c60: 2a00 0000 722b 0000 0072 2c00 0000 722d  *...r+...r,...r-
+00000c70: 0000 0072 2e00 0000 6993 0a00 00da 066c  ...r....i......l
+00000c80: 6179 6f75 744e 2905 da04 636f 6e6e da07  ayoutN)...conn..
+00000c90: 6164 6472 6573 73da 0a63 6f6d 6d69 746d  address..commitm
+00000ca0: 656e 74da 0a70 726f 6772 616d 5f69 64da  ent..program_id.
+00000cb0: 0672 6574 7572 6e63 0500 0000 0000 0000  .returnc........
+00000cc0: 0000 0000 0800 0000 0400 0000 c300 0000  ................
+00000cd0: 7348 0000 007c 016a 007c 027c 0364 018d  sH...|.j.|.|.d..
+00000ce0: 0249 0064 0048 007d 057c 056a 017d 067c  .I.d.H.}.|.j.}.|
+00000cf0: 0664 0075 0072 2664 0053 007c 066a 027c  .d.u.r&d.S.|.j.|
+00000d00: 046b 0372 3874 0364 0283 0182 017c 066a  .k.r8t.d.....|.j
+00000d10: 047d 077c 00a0 057c 07a1 0153 00a9 034e  .}.|...|...S...N
+00000d20: 2901 7246 0000 007a 2741 6363 6f75 6e74  ).rF...z'Account
+00000d30: 2064 6f65 7320 6e6f 7420 6265 6c6f 6e67   does not belong
+00000d40: 2074 6f20 7468 6973 2070 726f 6772 616d   to this program
+00000d50: 2906 da10 6765 745f 6163 636f 756e 745f  )...get_account_
+00000d60: 696e 666f da05 7661 6c75 65da 056f 776e  info..value..own
+00000d70: 6572 da0a 5661 6c75 6545 7272 6f72 da04  er..ValueError..
+00000d80: 6461 7461 da06 6465 636f 6465 2908 da03  data..decode)...
+00000d90: 636c 7372 4400 0000 7245 0000 0072 4600  clsrD...rE...rF.
+00000da0: 0000 7247 0000 00da 0472 6573 70da 0469  ..rG.....resp..i
+00000db0: 6e66 6fda 0a62 7974 6573 5f64 6174 6172  nfo..bytes_datar
+00000dc0: 3d00 0000 723d 0000 0072 3e00 0000 da05  =...r=...r>.....
+00000dd0: 6665 7463 687d 0000 0073 1000 0000 0008  fetch}...s......
+00000de0: 1401 0601 0801 0401 0a01 0801 0601 7a0d  ..............z.
+00000df0: 5072 6963 696e 672e 6665 7463 6829 0572  Pricing.fetch).r
+00000e00: 4400 0000 da09 6164 6472 6573 7365 7372  D.....addressesr
+00000e10: 4600 0000 7247 0000 0072 4800 0000 6305  F...rG...rH...c.
+00000e20: 0000 0000 0000 0000 0000 0008 0000 0006  ................
+00000e30: 0000 00c3 0000 0073 6200 0000 7400 7c01  .......sb...t.|.
+00000e40: 7c02 7c03 6401 8d03 4900 6400 4800 7d05  |.|.d...I.d.H.}.
+00000e50: 6700 7d06 7c05 4400 5d40 7d07 7c07 6400  g.}.|.D.]@}.|.d.
+00000e60: 7500 7234 7c06 a001 6400 a101 0100 711c  u.r4|...d.....q.
+00000e70: 7c07 6a02 6a03 7c04 6b03 7248 7404 6402  |.j.j.|.k.rHt.d.
+00000e80: 8301 8201 7c06 a001 7c00 a005 7c07 6a02  ....|...|...|.j.
+00000e90: 6a06 a101 a101 0100 711c 7c06 5300 7249  j.......q.|.S.rI
+00000ea0: 0000 0029 0772 0600 0000 da06 6170 7065  ...).r......appe
+00000eb0: 6e64 da07 6163 636f 756e 7472 4c00 0000  nd..accountrL...
+00000ec0: 724d 0000 0072 4f00 0000 724e 0000 0029  rM...rO...rN...)
+00000ed0: 0872 5000 0000 7244 0000 0072 5500 0000  .rP...rD...rU...
+00000ee0: 7246 0000 0072 4700 0000 da05 696e 666f  rF...rG.....info
+00000ef0: 73da 0372 6573 7252 0000 0072 3d00 0000  s..resrR...r=...
+00000f00: 723d 0000 0072 3e00 0000 da0e 6665 7463  r=...r>.....fetc
+00000f10: 685f 6d75 6c74 6970 6c65 8e00 0000 7314  h_multiple....s.
+00000f20: 0000 0000 0814 0104 0108 0108 010a 0102  ................
+00000f30: 010c 0108 0116 017a 1650 7269 6369 6e67  .......z.Pricing
+00000f40: 2e66 6574 6368 5f6d 756c 7469 706c 6529  .fetch_multiple)
+00000f50: 0272 4e00 0000 7248 0000 0063 0200 0000  .rN...rH...c....
+00000f60: 0000 0000 0000 0000 0300 0000 2300 0000  ............#...
+00000f70: 4300 0000 7346 0100 007c 0164 0074 0085  C...sF...|.d.t..
+00000f80: 0219 007c 006a 016b 0372 1a74 0264 0183  ...|.j.k.r.t.d..
+00000f90: 0182 0174 036a 04a0 057c 0174 0064 0085  ...t.j...|.t.d..
+00000fa0: 0219 00a1 017d 027c 007c 026a 067c 026a  .....}.|.|.j.|.j
+00000fb0: 077c 026a 087c 026a 097c 026a 0a74 0b74  .|.j.|.j.|.j.t.t
+00000fc0: 0c64 0264 0384 007c 026a 0d83 0283 0174  .d.d...|.j.....t
+00000fd0: 0b74 0c64 0464 0384 007c 026a 0e83 0283  .t.d.d...|.j....
+00000fe0: 0174 0b74 0c64 0564 0384 007c 026a 0f83  .t.t.d.d...|.j..
+00000ff0: 0283 0174 0b74 0c64 0664 0384 007c 026a  ...t.t.d.d...|.j
+00001000: 1083 0283 017c 026a 117c 026a 127c 026a  .....|.j.|.j.|.j
+00001010: 137c 026a 147c 026a 157c 026a 167c 026a  .|.j.|.j.|.j.|.j
+00001020: 177c 026a 187c 026a 197c 026a 1a74 0b74  .|.j.|.j.|.j.t.t
+00001030: 0c64 0764 0384 007c 026a 1b83 0283 0174  .d.d...|.j.....t
+00001040: 0b74 0c64 0864 0384 007c 026a 1c83 0283  .t.d.d...|.j....
+00001050: 0174 0b74 0c64 0964 0384 007c 026a 1d83  .t.t.d.d...|.j..
+00001060: 0283 0174 0b74 0c64 0a64 0384 007c 026a  ...t.t.d.d...|.j
+00001070: 1e83 0283 0174 0b74 0c64 0b64 0384 007c  .....t.t.d.d...|
+00001080: 026a 1f83 0283 0174 0b74 0c64 0c64 0384  .j.....t.t.d.d..
+00001090: 007c 026a 2083 0283 017c 026a 217c 026a  .|.j ....|.j!|.j
+000010a0: 227c 026a 237c 026a 247c 026a 257c 026a  "|.j#|.j$|.j%|.j
+000010b0: 267c 026a 277c 026a 2864 0d8d 2153 0029  &|.j'|.j(d..!S.)
+000010c0: 0e4e 7a2d 5468 6520 6469 7363 7269 6d69  .Nz-The discrimi
+000010d0: 6e61 746f 7220 666f 7220 7468 6973 2061  nator for this a
+000010e0: 6363 6f75 6e74 2069 7320 696e 7661 6c69  ccount is invali
+000010f0: 6463 0100 0000 0000 0000 0000 0000 0100  dc..............
+00001100: 0000 0300 0000 5300 0000 730e 0000 0074  ......S...s....t
+00001110: 006a 016a 02a0 037c 00a1 0153 00a9 014e  .j.j...|...S...N
+00001120: a904 720b 0000 0072 3500 0000 da0d 416e  ..r....r5.....An
+00001130: 6368 6f72 4465 6369 6d61 6cda 0c66 726f  chorDecimal..fro
+00001140: 6d5f 6465 636f 6465 64a9 01da 0469 7465  m_decoded....ite
+00001150: 6d72 3d00 0000 723d 0000 0072 3e00 0000  mr=...r=...r>...
+00001160: da08 3c6c 616d 6264 613e ae00 0000 f300  ..<lambda>......
+00001170: 0000 007a 2050 7269 6369 6e67 2e64 6563  ...z Pricing.dec
+00001180: 6f64 652e 3c6c 6f63 616c 733e 2e3c 6c61  ode.<locals>.<la
+00001190: 6d62 6461 3e63 0100 0000 0000 0000 0000  mbda>c..........
+000011a0: 0000 0100 0000 0300 0000 5300 0000 730e  ..........S...s.
+000011b0: 0000 0074 006a 016a 02a0 037c 00a1 0153  ...t.j.j...|...S
+000011c0: 0072 5b00 0000 725c 0000 0072 5f00 0000  .r[...r\...r_...
+000011d0: 723d 0000 0072 3d00 0000 723e 0000 0072  r=...r=...r>...r
+000011e0: 6100 0000 b400 0000 7262 0000 0063 0100  a.......rb...c..
+000011f0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00001200: 0000 5300 0000 730e 0000 0074 006a 016a  ..S...s....t.j.j
+00001210: 02a0 037c 00a1 0153 0072 5b00 0000 725c  ...|...S.r[...r\
+00001220: 0000 0072 5f00 0000 723d 0000 0072 3d00  ...r_...r=...r=.
+00001230: 0000 723e 0000 0072 6100 0000 ba00 0000  ..r>...ra.......
+00001240: 7262 0000 0063 0100 0000 0000 0000 0000  rb...c..........
+00001250: 0000 0100 0000 0300 0000 5300 0000 730e  ..........S...s.
+00001260: 0000 0074 006a 016a 02a0 037c 00a1 0153  ...t.j.j...|...S
+00001270: 0072 5b00 0000 725c 0000 0072 5f00 0000  .r[...r\...r_...
+00001280: 723d 0000 0072 3d00 0000 723e 0000 0072  r=...r=...r>...r
+00001290: 6100 0000 c000 0000 7262 0000 0063 0100  a.......rb...c..
+000012a0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+000012b0: 0000 5300 0000 730e 0000 0074 006a 016a  ..S...s....t.j.j
+000012c0: 02a0 037c 00a1 0153 0072 5b00 0000 a904  ...|...S.r[.....
+000012d0: 720b 0000 0072 2100 0000 da0e 5065 7270  r....r!.....Perp
+000012e0: 5061 7261 6d65 7465 7273 725e 0000 0072  Parametersr^...r
+000012f0: 5f00 0000 723d 0000 0072 3d00 0000 723e  _...r=...r=...r>
+00001300: 0000 0072 6100 0000 d000 0000 7262 0000  ...ra.......rb..
+00001310: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00001320: 0000 0300 0000 5300 0000 730e 0000 0074  ......S...s....t
+00001330: 006a 016a 02a0 037c 00a1 0153 0072 5b00  .j.j...|...S.r[.
+00001340: 0000 7263 0000 0072 5f00 0000 723d 0000  ..rc...r_...r=..
+00001350: 0072 3d00 0000 723e 0000 0072 6100 0000  .r=...r>...ra...
+00001360: d600 0000 7262 0000 0063 0100 0000 0000  ....rb...c......
+00001370: 0000 0000 0000 0100 0000 0300 0000 5300  ..............S.
+00001380: 0000 730e 0000 0074 006a 016a 02a0 037c  ..s....t.j.j...|
+00001390: 00a1 0153 0072 5b00 0000 a904 720b 0000  ...S.r[.....r...
+000013a0: 0072 2300 0000 da10 4d61 7267 696e 5061  .r#.....MarginPa
+000013b0: 7261 6d65 7465 7273 725e 0000 0072 5f00  rametersr^...r_.
+000013c0: 0000 723d 0000 0072 3d00 0000 723e 0000  ..r=...r=...r>..
+000013d0: 0072 6100 0000 dc00 0000 7262 0000 0063  .ra.......rb...c
+000013e0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000013f0: 0300 0000 5300 0000 730e 0000 0074 006a  ....S...s....t.j
+00001400: 016a 02a0 037c 00a1 0153 0072 5b00 0000  .j...|...S.r[...
+00001410: 7265 0000 0072 5f00 0000 723d 0000 0072  re...r_...r=...r
+00001420: 3d00 0000 723e 0000 0072 6100 0000 e200  =...r>...ra.....
+00001430: 0000 7262 0000 0063 0100 0000 0000 0000  ..rb...c........
+00001440: 0000 0000 0100 0000 0300 0000 5300 0000  ............S...
+00001450: 730e 0000 0074 006a 016a 02a0 037c 00a1  s....t.j.j...|..
+00001460: 0153 0072 5b00 0000 a904 720b 0000 0072  .S.r[.....r....r
+00001470: 3a00 0000 da07 5072 6f64 7563 7472 5e00  :.....Productr^.
+00001480: 0000 725f 0000 0072 3d00 0000 723d 0000  ..r_...r=...r=..
+00001490: 0072 3e00 0000 7261 0000 00e6 0000 0072  .r>...ra.......r
+000014a0: 6200 0000 6301 0000 0000 0000 0000 0000  b...c...........
+000014b0: 0001 0000 0003 0000 0053 0000 0073 0e00  .........S...s..
+000014c0: 0000 7400 6a01 6a02 a003 7c00 a101 5300  ..t.j.j...|...S.
+000014d0: 725b 0000 0072 6700 0000 725f 0000 0072  r[...rg...r_...r
+000014e0: 3d00 0000 723d 0000 0072 3e00 0000 7261  =...r=...r>...ra
+000014f0: 0000 00e9 0000 0072 6200 0000 a921 720e  .......rb....!r.
+00001500: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
+00001510: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00001520: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
+00001530: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00001540: 1b00 0000 721c 0000 0072 1d00 0000 721e  ....r....r....r.
+00001550: 0000 0072 1f00 0000 7220 0000 0072 2100  ...r....r ...r!.
+00001560: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
+00001570: 0072 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
+00001580: 7228 0000 0072 2900 0000 722a 0000 0072  r(...r)...r*...r
+00001590: 2b00 0000 722c 0000 0072 2d00 0000 722e  +...r,...r-...r.
+000015a0: 0000 0029 2972 0400 0000 7240 0000 0072  ...))r....r@...r
+000015b0: 0500 0000 723f 0000 0072 4300 0000 da05  ....r?...rC.....
+000015c0: 7061 7273 6572 0e00 0000 720f 0000 0072  parser....r....r
+000015d0: 1000 0000 7211 0000 0072 1200 0000 7234  ....r....r....r4
+000015e0: 0000 00da 036d 6170 7213 0000 0072 1400  .....mapr....r..
+000015f0: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00001600: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00001610: 721b 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
+00001620: 1e00 0000 721f 0000 0072 2000 0000 7221  ....r....r ...r!
+00001630: 0000 0072 2200 0000 7223 0000 0072 2400  ...r"...r#...r$.
+00001640: 0000 7225 0000 0072 2600 0000 7227 0000  ..r%...r&...r'..
+00001650: 0072 2800 0000 7229 0000 0072 2a00 0000  .r(...r)...r*...
+00001660: 722b 0000 0072 2c00 0000 722d 0000 0072  r+...r,...r-...r
+00001670: 2e00 0000 2903 7250 0000 0072 4e00 0000  ....).rP...rN...
+00001680: da03 6465 6372 3d00 0000 723d 0000 0072  ..decr=...r=...r
+00001690: 3e00 0000 724f 0000 00a1 0000 0073 a600  >...rO.......s..
+000016a0: 0000 0002 1201 0801 1401 0201 0401 0401  ................
+000016b0: 0401 0401 0401 0201 0201 0601 04fe 02ff  ................
+000016c0: 0206 0201 0201 0601 04fe 02ff 0206 0201  ................
+000016d0: 0201 0601 04fe 02ff 0206 0201 0201 0601  ................
+000016e0: 04fe 02ff 0206 0401 0401 0401 0401 0401  ................
+000016f0: 0401 0401 0401 0401 0401 0201 0201 0601  ................
+00001700: 04fe 02ff 0206 0201 0201 0601 04fe 02ff  ................
+00001710: 0206 0201 0201 0601 04fe 02ff 0206 0201  ................
+00001720: 0201 0601 04fe 02ff 0206 1201 0201 0201  ................
+00001730: 0601 04fe 02ff 0206 0401 0401 0401 0401  ................
+00001740: 0401 0401 0401 04b2 7a0e 5072 6963 696e  ........z.Pricin
+00001750: 672e 6465 636f 6465 2901 7248 0000 0063  g.decode).rH...c
+00001760: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001770: 2200 0000 4300 0000 73a2 0100 007c 006a  "...C...s....|.j
+00001780: 007c 006a 017c 006a 027c 006a 037c 006a  .|.j.|.j.|.j.|.j
+00001790: 0474 0574 0664 0164 0284 007c 006a 0783  .t.t.d.d...|.j..
+000017a0: 0283 0174 0574 0664 0364 0284 007c 006a  ...t.t.d.d...|.j
+000017b0: 0883 0283 0174 0574 0664 0464 0284 007c  .....t.t.d.d...|
+000017c0: 006a 0983 0283 0174 0574 0664 0564 0284  .j.....t.t.d.d..
+000017d0: 007c 006a 0a83 0283 017c 006a 0b7c 006a  .|.j.....|.j.|.j
+000017e0: 0c74 0574 0664 0664 0284 007c 006a 0d83  .t.t.d.d...|.j..
+000017f0: 0283 0174 0574 0664 0764 0284 007c 006a  ...t.t.d.d...|.j
+00001800: 0e83 0283 0174 0574 0664 0864 0284 007c  .....t.t.d.d...|
+00001810: 006a 0f83 0283 0174 0574 0664 0964 0284  .j.....t.t.d.d..
+00001820: 007c 006a 1083 0283 0174 0574 0664 0a64  .|.j.....t.t.d.d
+00001830: 0284 007c 006a 1183 0283 0174 0574 0664  ...|.j.....t.t.d
+00001840: 0b64 0284 007c 006a 1283 0283 0174 0574  .d...|.j.....t.t
+00001850: 0664 0c64 0284 007c 006a 1383 0283 0174  .d.d...|.j.....t
+00001860: 0574 0664 0d64 0284 007c 006a 1483 0283  .t.d.d...|.j....
+00001870: 0174 0574 0664 0e64 0284 007c 006a 1583  .t.t.d.d...|.j..
+00001880: 0283 0174 0574 0664 0f64 0284 007c 006a  ...t.t.d.d...|.j
+00001890: 1683 0283 0174 0574 0664 1064 0284 007c  .....t.t.d.d...|
+000018a0: 006a 1783 0283 0174 0574 0664 1164 0284  .j.....t.t.d.d..
+000018b0: 007c 006a 1883 0283 0174 0574 0664 1264  .|.j.....t.t.d.d
+000018c0: 0284 007c 006a 1983 0283 0174 0574 0664  ...|.j.....t.t.d
+000018d0: 1364 0284 007c 006a 1a83 0283 0174 0574  .d...|.j.....t.t
+000018e0: 0664 1464 0284 007c 006a 1b83 0283 0174  .d.d...|.j.....t
+000018f0: 0574 0664 1564 0284 007c 006a 1c83 0283  .t.d.d...|.j....
+00001900: 017c 006a 1d7c 006a 1e7c 006a 1f7c 006a  .|.j.|.j.|.j.|.j
+00001910: 207c 006a 217c 006a 2264 169c 2153 0029   |.j!|.j"d..!S.)
+00001920: 174e 6301 0000 0000 0000 0000 0000 0001  .Nc.............
+00001930: 0000 0002 0000 0053 0000 0073 0800 0000  .......S...s....
+00001940: 7c00 a000 a100 5300 725b 0000 00a9 01da  |.....S.r[......
+00001950: 0774 6f5f 6a73 6f6e 725f 0000 0072 3d00  .to_jsonr_...r=.
+00001960: 0000 723d 0000 0072 3e00 0000 7261 0000  ..r=...r>...ra..
+00001970: 00fe 0000 0072 6200 0000 7a21 5072 6963  .....rb...z!Pric
+00001980: 696e 672e 746f 5f6a 736f 6e2e 3c6c 6f63  ing.to_json.<loc
+00001990: 616c 733e 2e3c 6c61 6d62 6461 3e63 0100  als>.<lambda>c..
+000019a0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+000019b0: 0000 5300 0000 7308 0000 007c 00a0 00a1  ..S...s....|....
+000019c0: 0053 0072 5b00 0000 726d 0000 0072 5f00  .S.r[...rm...r_.
+000019d0: 0000 723d 0000 0072 3d00 0000 723e 0000  ..r=...r=...r>..
+000019e0: 0072 6100 0000 ff00 0000 7262 0000 0063  .ra.......rb...c
+000019f0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001a00: 0200 0000 5300 0000 7308 0000 007c 00a0  ....S...s....|..
+00001a10: 00a1 0053 0072 5b00 0000 726d 0000 0072  ...S.r[...rm...r
+00001a20: 5f00 0000 723d 0000 0072 3d00 0000 723e  _...r=...r=...r>
+00001a30: 0000 0072 6100 0000 0001 0000 7262 0000  ...ra.......rb..
+00001a40: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00001a50: 0000 0200 0000 5300 0000 7308 0000 007c  ......S...s....|
+00001a60: 00a0 00a1 0053 0072 5b00 0000 726d 0000  .....S.r[...rm..
+00001a70: 0072 5f00 0000 723d 0000 0072 3d00 0000  .r_...r=...r=...
+00001a80: 723e 0000 0072 6100 0000 0101 0000 7262  r>...ra.......rb
+00001a90: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001aa0: 0100 0000 0200 0000 5300 0000 7308 0000  ........S...s...
+00001ab0: 0074 007c 0083 0153 0072 5b00 0000 a901  .t.|...S.r[.....
+00001ac0: 7237 0000 0072 5f00 0000 723d 0000 0072  r7...r_...r=...r
+00001ad0: 3d00 0000 723e 0000 0072 6100 0000 0401  =...r>...ra.....
+00001ae0: 0000 7262 0000 0063 0100 0000 0000 0000  ..rb...c........
+00001af0: 0000 0000 0100 0000 0200 0000 5300 0000  ............S...
+00001b00: 7308 0000 0074 007c 0083 0153 0072 5b00  s....t.|...S.r[.
+00001b10: 0000 726f 0000 0072 5f00 0000 723d 0000  ..ro...r_...r=..
+00001b20: 0072 3d00 0000 723e 0000 0072 6100 0000  .r=...r>...ra...
+00001b30: 0501 0000 7262 0000 0063 0100 0000 0000  ....rb...c......
+00001b40: 0000 0000 0000 0100 0000 0200 0000 5300  ..............S.
+00001b50: 0000 7308 0000 0074 007c 0083 0153 0072  ..s....t.|...S.r
+00001b60: 5b00 0000 726f 0000 0072 5f00 0000 723d  [...ro...r_...r=
+00001b70: 0000 0072 3d00 0000 723e 0000 0072 6100  ...r=...r>...ra.
+00001b80: 0000 0601 0000 7262 0000 0063 0100 0000  ......rb...c....
+00001b90: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00001ba0: 5300 0000 7308 0000 0074 007c 0083 0153  S...s....t.|...S
+00001bb0: 0072 5b00 0000 726f 0000 0072 5f00 0000  .r[...ro...r_...
+00001bc0: 723d 0000 0072 3d00 0000 723e 0000 0072  r=...r=...r>...r
+00001bd0: 6100 0000 0701 0000 7262 0000 0063 0100  a.......rb...c..
+00001be0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00001bf0: 0000 5300 0000 7308 0000 0074 007c 0083  ..S...s....t.|..
+00001c00: 0153 0072 5b00 0000 726f 0000 0072 5f00  .S.r[...ro...r_.
+00001c10: 0000 723d 0000 0072 3d00 0000 723e 0000  ..r=...r=...r>..
+00001c20: 0072 6100 0000 0801 0000 7262 0000 0063  .ra.......rb...c
+00001c30: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001c40: 0200 0000 5300 0000 7308 0000 0074 007c  ....S...s....t.|
+00001c50: 0083 0153 0072 5b00 0000 726f 0000 0072  ...S.r[...ro...r
+00001c60: 5f00 0000 723d 0000 0072 3d00 0000 723e  _...r=...r=...r>
+00001c70: 0000 0072 6100 0000 0901 0000 7262 0000  ...ra.......rb..
+00001c80: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00001c90: 0000 0200 0000 5300 0000 7308 0000 0074  ......S...s....t
+00001ca0: 007c 0083 0153 0072 5b00 0000 726f 0000  .|...S.r[...ro..
+00001cb0: 0072 5f00 0000 723d 0000 0072 3d00 0000  .r_...r=...r=...
+00001cc0: 723e 0000 0072 6100 0000 0a01 0000 7262  r>...ra.......rb
+00001cd0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001ce0: 0100 0000 0200 0000 5300 0000 7308 0000  ........S...s...
+00001cf0: 0074 007c 0083 0153 0072 5b00 0000 726f  .t.|...S.r[...ro
+00001d00: 0000 0072 5f00 0000 723d 0000 0072 3d00  ...r_...r=...r=.
+00001d10: 0000 723e 0000 0072 6100 0000 0b01 0000  ..r>...ra.......
+00001d20: 7262 0000 0063 0100 0000 0000 0000 0000  rb...c..........
+00001d30: 0000 0100 0000 0200 0000 5300 0000 7308  ..........S...s.
+00001d40: 0000 007c 00a0 00a1 0053 0072 5b00 0000  ...|.....S.r[...
+00001d50: 726d 0000 0072 5f00 0000 723d 0000 0072  rm...r_...r=...r
+00001d60: 3d00 0000 723e 0000 0072 6100 0000 0c01  =...r>...ra.....
+00001d70: 0000 7262 0000 0063 0100 0000 0000 0000  ..rb...c........
+00001d80: 0000 0000 0100 0000 0200 0000 5300 0000  ............S...
+00001d90: 7308 0000 007c 00a0 00a1 0053 0072 5b00  s....|.....S.r[.
+00001da0: 0000 726d 0000 0072 5f00 0000 723d 0000  ..rm...r_...r=..
+00001db0: 0072 3d00 0000 723e 0000 0072 6100 0000  .r=...r>...ra...
+00001dc0: 0d01 0000 7262 0000 0063 0100 0000 0000  ....rb...c......
+00001dd0: 0000 0000 0000 0100 0000 0200 0000 5300  ..............S.
+00001de0: 0000 7308 0000 007c 00a0 00a1 0053 0072  ..s....|.....S.r
+00001df0: 5b00 0000 726d 0000 0072 5f00 0000 723d  [...rm...r_...r=
+00001e00: 0000 0072 3d00 0000 723e 0000 0072 6100  ...r=...r>...ra.
+00001e10: 0000 0e01 0000 7262 0000 0063 0100 0000  ......rb...c....
+00001e20: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00001e30: 5300 0000 7308 0000 007c 00a0 00a1 0053  S...s....|.....S
+00001e40: 0072 5b00 0000 726d 0000 0072 5f00 0000  .r[...rm...r_...
+00001e50: 723d 0000 0072 3d00 0000 723e 0000 0072  r=...r=...r>...r
+00001e60: 6100 0000 0f01 0000 7262 0000 0063 0100  a.......rb...c..
+00001e70: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00001e80: 0000 5300 0000 7308 0000 007c 00a0 00a1  ..S...s....|....
+00001e90: 0053 0072 5b00 0000 726d 0000 0072 5f00  .S.r[...rm...r_.
+00001ea0: 0000 723d 0000 0072 3d00 0000 723e 0000  ..r=...r=...r>..
+00001eb0: 0072 6100 0000 1001 0000 7262 0000 0063  .ra.......rb...c
+00001ec0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001ed0: 0200 0000 5300 0000 7308 0000 007c 00a0  ....S...s....|..
+00001ee0: 00a1 0053 0072 5b00 0000 726d 0000 0072  ...S.r[...rm...r
+00001ef0: 5f00 0000 723d 0000 0072 3d00 0000 723e  _...r=...r=...r>
+00001f00: 0000 0072 6100 0000 1101 0000 7262 0000  ...ra.......rb..
+00001f10: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00001f20: 0000 0200 0000 5300 0000 7308 0000 0074  ......S...s....t
+00001f30: 007c 0083 0153 0072 5b00 0000 726f 0000  .|...S.r[...ro..
+00001f40: 0072 5f00 0000 723d 0000 0072 3d00 0000  .r_...r=...r=...
+00001f50: 723e 0000 0072 6100 0000 1201 0000 7262  r>...ra.......rb
+00001f60: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001f70: 0100 0000 0200 0000 5300 0000 7308 0000  ........S...s...
+00001f80: 0074 007c 0083 0153 0072 5b00 0000 726f  .t.|...S.r[...ro
+00001f90: 0000 0072 5f00 0000 723d 0000 0072 3d00  ...r_...r=...r=.
+00001fa0: 0000 723e 0000 0072 6100 0000 1301 0000  ..r>...ra.......
+00001fb0: 7262 0000 0072 6900 0000 2923 720e 0000  rb...ri...)#r...
+00001fc0: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
+00001fd0: 7212 0000 0072 3400 0000 726b 0000 0072  r....r4...rk...r
+00001fe0: 1300 0000 7214 0000 0072 1500 0000 7216  ....r....r....r.
+00001ff0: 0000 0072 1700 0000 7218 0000 0072 1900  ...r....r....r..
+00002000: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+00002010: 0072 1d00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00002020: 7220 0000 0072 2100 0000 7222 0000 0072  r ...r!...r"...r
+00002030: 2300 0000 7224 0000 0072 2500 0000 7226  #...r$...r%...r&
+00002040: 0000 0072 2700 0000 7228 0000 0072 2900  ...r'...r(...r).
+00002050: 0000 722a 0000 0072 2b00 0000 722c 0000  ..r*...r+...r,..
+00002060: 0072 2d00 0000 722e 0000 0029 01da 0473  .r-...r....)...s
+00002070: 656c 6672 3d00 0000 723d 0000 0072 3e00  elfr=...r=...r>.
+00002080: 0000 726e 0000 00f7 0000 0073 4400 0000  ..rn.......sD...
+00002090: 0002 0401 0401 0401 0401 0401 1201 1201  ................
+000020a0: 1201 1201 0401 0401 1201 1201 1201 1201  ................
+000020b0: 1201 1201 1201 1201 1201 1201 1201 1201  ................
+000020c0: 1201 1201 1201 1201 0401 0401 0401 0401  ................
+000020d0: 0401 04df 7a0f 5072 6963 696e 672e 746f  ....z.Pricing.to
+000020e0: 5f6a 736f 6e29 02da 036f 626a 7248 0000  _json)...objrH..
+000020f0: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+00002100: 0000 2300 0000 4300 0000 73e6 0100 007c  ..#...C...s....|
+00002110: 007c 0164 0119 007c 0164 0219 007c 0164  .|.d...|.d...|.d
+00002120: 0319 007c 0164 0419 007c 0164 0519 0074  ...|.d...|.d...t
+00002130: 0074 0164 0664 0784 007c 0164 0819 0083  .t.d.d...|.d....
+00002140: 0283 0174 0074 0164 0964 0784 007c 0164  ...t.t.d.d...|.d
+00002150: 0a19 0083 0283 0174 0074 0164 0b64 0784  .......t.t.d.d..
+00002160: 007c 0164 0c19 0083 0283 0174 0074 0164  .|.d.......t.t.d
+00002170: 0d64 0784 007c 0164 0e19 0083 0283 017c  .d...|.d.......|
+00002180: 0164 0f19 007c 0164 1019 0074 0074 0164  .d...|.d...t.t.d
+00002190: 1164 0784 007c 0164 1219 0083 0283 0174  .d...|.d.......t
+000021a0: 0074 0164 1364 0784 007c 0164 1419 0083  .t.d.d...|.d....
+000021b0: 0283 0174 0074 0164 1564 0784 007c 0164  ...t.t.d.d...|.d
+000021c0: 1619 0083 0283 0174 0074 0164 1764 0784  .......t.t.d.d..
+000021d0: 007c 0164 1819 0083 0283 0174 0074 0164  .|.d.......t.t.d
+000021e0: 1964 0784 007c 0164 1a19 0083 0283 0174  .d...|.d.......t
+000021f0: 0074 0164 1b64 0784 007c 0164 1c19 0083  .t.d.d...|.d....
+00002200: 0283 0174 0074 0164 1d64 0784 007c 0164  ...t.t.d.d...|.d
+00002210: 1e19 0083 0283 0174 0074 0164 1f64 0784  .......t.t.d.d..
+00002220: 007c 0164 2019 0083 0283 0174 0074 0164  .|.d ......t.t.d
+00002230: 2164 0784 007c 0164 2219 0083 0283 0174  !d...|.d"......t
+00002240: 0074 0164 2364 0784 007c 0164 2419 0083  .t.d#d...|.d$...
+00002250: 0283 0174 0074 0164 2564 0784 007c 0164  ...t.t.d%d...|.d
+00002260: 2619 0083 0283 0174 0074 0164 2764 0784  &......t.t.d'd..
+00002270: 007c 0164 2819 0083 0283 0174 0074 0164  .|.d(......t.t.d
+00002280: 2964 0784 007c 0164 2a19 0083 0283 0174  )d...|.d*......t
+00002290: 0074 0164 2b64 0784 007c 0164 2c19 0083  .t.d+d...|.d,...
+000022a0: 0283 0174 0074 0164 2d64 0784 007c 0164  ...t.t.d-d...|.d
+000022b0: 2e19 0083 0283 0174 0074 0164 2f64 0784  .......t.t.d/d..
+000022c0: 007c 0164 3019 0083 0283 017c 0164 3119  .|.d0......|.d1.
+000022d0: 007c 0164 3219 007c 0164 3319 007c 0164  .|.d2..|.d3..|.d
+000022e0: 3419 007c 0164 3519 007c 0164 3619 0064  4..|.d5..|.d6..d
+000022f0: 378d 2153 0029 384e 720e 0000 0072 0f00  7.!S.)8Nr....r..
+00002300: 0000 7210 0000 0072 1100 0000 7212 0000  ..r....r....r...
+00002310: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00002320: 0000 0300 0000 5300 0000 730e 0000 0074  ......S...s....t
+00002330: 006a 016a 02a0 037c 00a1 0153 0072 5b00  .j.j...|...S.r[.
+00002340: 0000 a904 720b 0000 0072 3500 0000 725d  ....r....r5...r]
+00002350: 0000 00da 0966 726f 6d5f 6a73 6f6e 725f  .....from_jsonr_
+00002360: 0000 0072 3d00 0000 723d 0000 0072 3e00  ...r=...r=...r>.
+00002370: 0000 7261 0000 0026 0100 0072 6200 0000  ..ra...&...rb...
+00002380: 7a23 5072 6963 696e 672e 6672 6f6d 5f6a  z#Pricing.from_j
+00002390: 736f 6e2e 3c6c 6f63 616c 733e 2e3c 6c61  son.<locals>.<la
+000023a0: 6d62 6461 3e72 1300 0000 6301 0000 0000  mbda>r....c.....
+000023b0: 0000 0000 0000 0001 0000 0003 0000 0053  ...............S
+000023c0: 0000 0073 0e00 0000 7400 6a01 6a02 a003  ...s....t.j.j...
+000023d0: 7c00 a101 5300 725b 0000 0072 7200 0000  |...S.r[...rr...
+000023e0: 725f 0000 0072 3d00 0000 723d 0000 0072  r_...r=...r=...r
+000023f0: 3e00 0000 7261 0000 002c 0100 0072 6200  >...ra...,...rb.
+00002400: 0000 7214 0000 0063 0100 0000 0000 0000  ..r....c........
+00002410: 0000 0000 0100 0000 0300 0000 5300 0000  ............S...
+00002420: 730e 0000 0074 006a 016a 02a0 037c 00a1  s....t.j.j...|..
+00002430: 0153 0072 5b00 0000 7272 0000 0072 5f00  .S.r[...rr...r_.
+00002440: 0000 723d 0000 0072 3d00 0000 723e 0000  ..r=...r=...r>..
+00002450: 0072 6100 0000 3201 0000 7262 0000 0072  .ra...2...rb...r
+00002460: 1500 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00002470: 0001 0000 0003 0000 0053 0000 0073 0e00  .........S...s..
+00002480: 0000 7400 6a01 6a02 a003 7c00 a101 5300  ..t.j.j...|...S.
+00002490: 725b 0000 0072 7200 0000 725f 0000 0072  r[...rr...r_...r
+000024a0: 3d00 0000 723d 0000 0072 3e00 0000 7261  =...r=...r>...ra
+000024b0: 0000 0038 0100 0072 6200 0000 7216 0000  ...8...rb...r...
+000024c0: 0072 1700 0000 7218 0000 0063 0100 0000  .r....r....c....
+000024d0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+000024e0: 5300 0000 730a 0000 0074 00a0 017c 00a1  S...s....t...|..
+000024f0: 0153 0072 5b00 0000 a902 7209 0000 00da  .S.r[.....r.....
+00002500: 0b66 726f 6d5f 7374 7269 6e67 725f 0000  .from_stringr_..
+00002510: 0072 3d00 0000 723d 0000 0072 3e00 0000  .r=...r=...r>...
+00002520: 7261 0000 003e 0100 0072 6200 0000 7219  ra...>...rb...r.
+00002530: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00002540: 0100 0000 0300 0000 5300 0000 730a 0000  ........S...s...
+00002550: 0074 00a0 017c 00a1 0153 0072 5b00 0000  .t...|...S.r[...
+00002560: 7274 0000 0072 5f00 0000 723d 0000 0072  rt...r_...r=...r
+00002570: 3d00 0000 723e 0000 0072 6100 0000 3f01  =...r>...ra...?.
+00002580: 0000 7262 0000 0072 1a00 0000 6301 0000  ..rb...r....c...
+00002590: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+000025a0: 0053 0000 0073 0a00 0000 7400 a001 7c00  .S...s....t...|.
+000025b0: a101 5300 725b 0000 0072 7400 0000 725f  ..S.r[...rt...r_
+000025c0: 0000 0072 3d00 0000 723d 0000 0072 3e00  ...r=...r=...r>.
+000025d0: 0000 7261 0000 0040 0100 0072 6200 0000  ..ra...@...rb...
+000025e0: 721b 0000 0063 0100 0000 0000 0000 0000  r....c..........
+000025f0: 0000 0100 0000 0300 0000 5300 0000 730a  ..........S...s.
+00002600: 0000 0074 00a0 017c 00a1 0153 0072 5b00  ...t...|...S.r[.
+00002610: 0000 7274 0000 0072 5f00 0000 723d 0000  ..rt...r_...r=..
+00002620: 0072 3d00 0000 723e 0000 0072 6100 0000  .r=...r>...ra...
+00002630: 4301 0000 7262 0000 0072 1c00 0000 6301  C...rb...r....c.
+00002640: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00002650: 0000 0053 0000 0073 0a00 0000 7400 a001  ...S...s....t...
+00002660: 7c00 a101 5300 725b 0000 0072 7400 0000  |...S.r[...rt...
+00002670: 725f 0000 0072 3d00 0000 723d 0000 0072  r_...r=...r=...r
+00002680: 3e00 0000 7261 0000 0047 0100 0072 6200  >...ra...G...rb.
+00002690: 0000 721d 0000 0063 0100 0000 0000 0000  ..r....c........
+000026a0: 0000 0000 0100 0000 0300 0000 5300 0000  ............S...
+000026b0: 730a 0000 0074 00a0 017c 00a1 0153 0072  s....t...|...S.r
+000026c0: 5b00 0000 7274 0000 0072 5f00 0000 723d  [...rt...r_...r=
+000026d0: 0000 0072 3d00 0000 723e 0000 0072 6100  ...r=...r>...ra.
+000026e0: 0000 4801 0000 7262 0000 0072 1e00 0000  ..H...rb...r....
+000026f0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00002700: 0003 0000 0053 0000 0073 0a00 0000 7400  .....S...s....t.
+00002710: a001 7c00 a101 5300 725b 0000 0072 7400  ..|...S.r[...rt.
+00002720: 0000 725f 0000 0072 3d00 0000 723d 0000  ..r_...r=...r=..
+00002730: 0072 3e00 0000 7261 0000 0049 0100 0072  .r>...ra...I...r
+00002740: 6200 0000 721f 0000 0063 0100 0000 0000  b...r....c......
+00002750: 0000 0000 0000 0100 0000 0300 0000 5300  ..............S.
+00002760: 0000 730a 0000 0074 00a0 017c 00a1 0153  ..s....t...|...S
+00002770: 0072 5b00 0000 7274 0000 0072 5f00 0000  .r[...rt...r_...
+00002780: 723d 0000 0072 3d00 0000 723e 0000 0072  r=...r=...r>...r
+00002790: 6100 0000 4c01 0000 7262 0000 0072 2000  a...L...rb...r .
+000027a0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
+000027b0: 0000 0003 0000 0053 0000 0073 0e00 0000  .......S...s....
+000027c0: 7400 6a01 6a02 a003 7c00 a101 5300 725b  t.j.j...|...S.r[
+000027d0: 0000 00a9 0472 0b00 0000 7221 0000 0072  .....r....r!...r
+000027e0: 6400 0000 7273 0000 0072 5f00 0000 723d  d...rs...r_...r=
+000027f0: 0000 0072 3d00 0000 723e 0000 0072 6100  ...r=...r>...ra.
+00002800: 0000 5201 0000 7262 0000 0072 2100 0000  ..R...rb...r!...
+00002810: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00002820: 0003 0000 0053 0000 0073 0e00 0000 7400  .....S...s....t.
+00002830: 6a01 6a02 a003 7c00 a101 5300 725b 0000  j.j...|...S.r[..
+00002840: 0072 7600 0000 725f 0000 0072 3d00 0000  .rv...r_...r=...
+00002850: 723d 0000 0072 3e00 0000 7261 0000 0058  r=...r>...ra...X
+00002860: 0100 0072 6200 0000 7222 0000 0063 0100  ...rb...r"...c..
+00002870: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00002880: 0000 5300 0000 730e 0000 0074 006a 016a  ..S...s....t.j.j
+00002890: 02a0 037c 00a1 0153 0072 5b00 0000 a904  ...|...S.r[.....
+000028a0: 720b 0000 0072 2300 0000 7266 0000 0072  r....r#...rf...r
+000028b0: 7300 0000 725f 0000 0072 3d00 0000 723d  s...r_...r=...r=
+000028c0: 0000 0072 3e00 0000 7261 0000 005e 0100  ...r>...ra...^..
+000028d0: 0072 6200 0000 7223 0000 0063 0100 0000  .rb...r#...c....
+000028e0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+000028f0: 5300 0000 730e 0000 0074 006a 016a 02a0  S...s....t.j.j..
+00002900: 037c 00a1 0153 0072 5b00 0000 7277 0000  .|...S.r[...rw..
+00002910: 0072 5f00 0000 723d 0000 0072 3d00 0000  .r_...r=...r=...
+00002920: 723e 0000 0072 6100 0000 6401 0000 7262  r>...ra...d...rb
+00002930: 0000 0072 2400 0000 6301 0000 0000 0000  ...r$...c.......
+00002940: 0000 0000 0001 0000 0003 0000 0053 0000  .............S..
+00002950: 0073 0e00 0000 7400 6a01 6a02 a003 7c00  .s....t.j.j...|.
+00002960: a101 5300 725b 0000 00a9 0472 0b00 0000  ..S.r[.....r....
+00002970: 723a 0000 0072 6800 0000 7273 0000 0072  r:...rh...rs...r
+00002980: 5f00 0000 723d 0000 0072 3d00 0000 723e  _...r=...r=...r>
+00002990: 0000 0072 6100 0000 6801 0000 7262 0000  ...ra...h...rb..
+000029a0: 0072 2500 0000 6301 0000 0000 0000 0000  .r%...c.........
+000029b0: 0000 0001 0000 0003 0000 0053 0000 0073  ...........S...s
+000029c0: 0e00 0000 7400 6a01 6a02 a003 7c00 a101  ....t.j.j...|...
+000029d0: 5300 725b 0000 0072 7800 0000 725f 0000  S.r[...rx...r_..
+000029e0: 0072 3d00 0000 723d 0000 0072 3e00 0000  .r=...r=...r>...
+000029f0: 7261 0000 006b 0100 0072 6200 0000 7226  ra...k...rb...r&
+00002a00: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00002a10: 0100 0000 0300 0000 5300 0000 730a 0000  ........S...s...
+00002a20: 0074 00a0 017c 00a1 0153 0072 5b00 0000  .t...|...S.r[...
+00002a30: 7274 0000 0072 5f00 0000 723d 0000 0072  rt...r_...r=...r
+00002a40: 3d00 0000 723e 0000 0072 6100 0000 6f01  =...r>...ra...o.
+00002a50: 0000 7262 0000 0072 2700 0000 6301 0000  ..rb...r'...c...
+00002a60: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00002a70: 0053 0000 0073 0a00 0000 7400 a001 7c00  .S...s....t...|.
+00002a80: a101 5300 725b 0000 0072 7400 0000 725f  ..S.r[...rt...r_
+00002a90: 0000 0072 3d00 0000 723d 0000 0072 3e00  ...r=...r=...r>.
+00002aa0: 0000 7261 0000 0072 0100 0072 6200 0000  ..ra...r...rb...
+00002ab0: 7228 0000 0072 2900 0000 722a 0000 0072  r(...r)...r*...r
+00002ac0: 2b00 0000 722c 0000 0072 2d00 0000 722e  +...r,...r-...r.
+00002ad0: 0000 0072 6900 0000 2902 7234 0000 0072  ...ri...).r4...r
+00002ae0: 6b00 0000 2902 7250 0000 0072 7100 0000  k...).rP...rq...
+00002af0: 723d 0000 0072 3d00 0000 723e 0000 0072  r=...r=...r>...r
+00002b00: 7300 0000 1c01 0000 73be 0000 0000 0202  s.......s.......
+00002b10: 0106 0106 0106 0106 0106 0102 0102 0106  ................
+00002b20: 0106 fe02 ff02 0602 0102 0106 0106 fe02  ................
+00002b30: ff02 0602 0102 0106 0106 fe02 ff02 0602  ................
+00002b40: 0102 0106 0106 fe02 ff02 0606 0106 0114  ................
+00002b50: 0114 0114 0102 0102 0106 0106 fe02 ff02  ................
+00002b60: 0614 0114 0114 0102 0102 0106 0106 fe02  ................
+00002b70: ff02 0602 0102 0106 0106 fe02 ff02 0602  ................
+00002b80: 0102 0106 0106 fe02 ff02 0602 0102 0106  ................
+00002b90: 0106 fe02 ff02 0602 0102 0106 0106 fe02  ................
 00002ba0: ff02 0614 0102 0102 0106 0106 fe02 ff02  ................
-00002bb0: 0606 0106 0106 0106 0106 0106 a37a 1150  .............z.P
-00002bc0: 7269 6369 6e67 2e66 726f 6d5f 6a73 6f6e  ricing.from_json
-00002bd0: 2929 722f 0000 0072 3000 0000 7231 0000  ))r/...r0...r1..
-00002be0: 0072 4000 0000 da06 7479 7069 6e67 da08  .r@.....typing..
-00002bf0: 436c 6173 7356 6172 7233 0000 00da 0562  ClassVarr3.....b
-00002c00: 6f72 7368 da07 4353 7472 7563 74da 0255  orsh..CStruct..U
-00002c10: 38da 0355 3634 720b 0000 0072 3500 0000  8..U64r....r5...
-00002c20: 725d 0000 0072 4300 0000 7203 0000 0072  r]...rC...r....r
-00002c30: 2100 0000 7264 0000 0072 2300 0000 7266  !...rd...r#...rf
-00002c40: 0000 0072 3a00 0000 7268 0000 00da 0349  ...r:...rh.....I
-00002c50: 3634 da04 426f 6f6c 7232 0000 0072 3400  64..Boolr2...r4.
-00002c60: 0000 7209 0000 0072 3c00 0000 da0b 636c  ..r....r<.....cl
-00002c70: 6173 736d 6574 686f 6472 0c00 0000 7207  assmethodr....r.
-00002c80: 0000 00da 084f 7074 696f 6e61 6c72 0800  .....Optionalr..
-00002c90: 0000 7254 0000 00da 044c 6973 7472 5a00  ..rT.....ListrZ.
-00002ca0: 0000 da05 6279 7465 7372 4f00 0000 720d  ....bytesrO...r.
-00002cb0: 0000 0072 6e00 0000 7273 0000 0072 3d00  ...rn...rs...r=.
-00002cc0: 0000 723d 0000 0072 3d00 0000 723e 0000  ..r=...r=...r>..
-00002cd0: 0072 3f00 0000 3500 0000 73bc 0000 000a  .r?...5...s.....
-00002ce0: 020e 0104 0108 010c 010c 010c 010c 0110  ................
-00002cf0: 0110 0110 0110 010c 010c 010a 010a 010a  ................
-00002d00: 010a 010a 010a 010a 010a 0110 0110 0110  ................
-00002d10: 0110 0110 0110 010a 010a 0108 0108 0108  ................
-00002d20: 010c 010c 010c df0e 2308 010c 010c 010c  ........#.......
-00002d30: 010c 0110 0110 0110 0110 010c 010c 010c  ................
-00002d40: 010c 010c 010c 010c 010c 010c 010c 0110  ................
-00002d50: 0110 0110 0110 0110 0110 010c 010c 0108  ................
-00002d60: 0108 0108 010c 010c 010c 0202 0502 0102  ................
-00002d70: fb02 0202 0102 0108 0102 0108 fa0e 1002  ................
-00002d80: 0502 0102 fb02 0202 0106 0108 0102 010e  ................
-00002d90: fa0e 1202 0112 550e 2502 0172 3f00 0000  ......U.%..r?...
-00002da0: 291a 7279 0000 00da 0b64 6174 6163 6c61  ).ry.....datacla
-00002db0: 7373 6573 7202 0000 00da 0f62 6f72 7368  ssesr......borsh
-00002dc0: 5f63 6f6e 7374 7275 6374 727b 0000 00da  _constructr{....
-00002dd0: 1861 6e63 686f 7270 792e 626f 7273 685f  .anchorpy.borsh_
-00002de0: 6578 7465 6e73 696f 6e72 0300 0000 da17  extensionr......
-00002df0: 616e 6368 6f72 7079 2e63 6f64 6572 2e61  anchorpy.coder.a
-00002e00: 6363 6f75 6e74 7372 0400 0000 5a0e 616e  ccountsr....Z.an
-00002e10: 6368 6f72 7079 2e65 7272 6f72 7205 0000  chorpy.errorr...
-00002e20: 005a 1261 6e63 686f 7270 792e 7574 696c  .Z.anchorpy.util
-00002e30: 732e 7270 6372 0600 0000 da14 736f 6c61  s.rpcr......sola
-00002e40: 6e61 2e72 7063 2e61 7379 6e63 5f61 7069  na.rpc.async_api
-00002e50: 7207 0000 00da 1573 6f6c 616e 612e 7270  r......solana.rp
-00002e60: 632e 636f 6d6d 6974 6d65 6e74 7208 0000  c.commitmentr...
-00002e70: 00da 0e73 6f6c 6465 7273 2e70 7562 6b65  ...solders.pubke
-00002e80: 7972 0900 0000 da00 720b 0000 0072 4700  yr......r....rG.
-00002e90: 0000 720c 0000 00da 0954 7970 6564 4469  ..r......TypedDi
-00002ea0: 6374 720d 0000 0072 3f00 0000 723d 0000  ctr....r?...r=..
-00002eb0: 0072 3d00 0000 723d 0000 0072 3e00 0000  .r=...r=...r>...
-00002ec0: da08 3c6d 6f64 756c 653e 0100 0000 731c  ..<module>....s.
-00002ed0: 0000 0008 010c 0208 010c 010c 010c 010c  ................
-00002ee0: 010c 010c 010c 020c 010c 0312 2402 01    ............$..
+00002bb0: 0614 0102 0102 0106 0106 fe02 ff02 0606  ................
+00002bc0: 0106 0106 0106 0106 0106 a37a 1150 7269  ...........z.Pri
+00002bd0: 6369 6e67 2e66 726f 6d5f 6a73 6f6e 2929  cing.from_json))
+00002be0: 722f 0000 0072 3000 0000 7231 0000 0072  r/...r0...r1...r
+00002bf0: 4000 0000 da06 7479 7069 6e67 da08 436c  @.....typing..Cl
+00002c00: 6173 7356 6172 7233 0000 00da 0562 6f72  assVarr3.....bor
+00002c10: 7368 da07 4353 7472 7563 74da 0255 38da  sh..CStruct..U8.
+00002c20: 0355 3634 720b 0000 0072 3500 0000 725d  .U64r....r5...r]
+00002c30: 0000 0072 4300 0000 7203 0000 0072 2100  ...rC...r....r!.
+00002c40: 0000 7264 0000 0072 2300 0000 7266 0000  ..rd...r#...rf..
+00002c50: 0072 3a00 0000 7268 0000 00da 0349 3634  .r:...rh.....I64
+00002c60: da04 426f 6f6c 7232 0000 0072 3400 0000  ..Boolr2...r4...
+00002c70: 7209 0000 0072 3c00 0000 da0b 636c 6173  r....r<.....clas
+00002c80: 736d 6574 686f 6472 0c00 0000 7207 0000  smethodr....r...
+00002c90: 00da 084f 7074 696f 6e61 6c72 0800 0000  ...Optionalr....
+00002ca0: 7254 0000 00da 044c 6973 7472 5a00 0000  rT.....ListrZ...
+00002cb0: da05 6279 7465 7372 4f00 0000 720d 0000  ..bytesrO...r...
+00002cc0: 0072 6e00 0000 7273 0000 0072 3d00 0000  .rn...rs...r=...
+00002cd0: 723d 0000 0072 3d00 0000 723e 0000 0072  r=...r=...r>...r
+00002ce0: 3f00 0000 3500 0000 73bc 0000 000a 020e  ?...5...s.......
+00002cf0: 0104 0108 010c 010c 010c 010c 0110 0110  ................
+00002d00: 0110 0110 010c 010c 010a 010a 010a 010a  ................
+00002d10: 010a 010a 010a 010a 0110 0110 0110 0110  ................
+00002d20: 0110 0110 010a 010a 0108 0108 0108 010c  ................
+00002d30: 010c 010c df0e 2308 010c 010c 010c 010c  ......#.........
+00002d40: 0110 0110 0110 0110 010c 010c 010c 010c  ................
+00002d50: 010c 010c 010c 010c 010c 010c 0110 0110  ................
+00002d60: 0110 0110 0110 0110 010c 010c 0108 0108  ................
+00002d70: 0108 010c 010c 010c 0202 0502 0102 fb02  ................
+00002d80: 0202 0102 0108 0102 0108 fa0e 1002 0502  ................
+00002d90: 0102 fb02 0202 0106 0108 0102 010e fa0e  ................
+00002da0: 1202 0112 550e 2502 0172 3f00 0000 291a  ....U.%..r?...).
+00002db0: 7279 0000 00da 0b64 6174 6163 6c61 7373  ry.....dataclass
+00002dc0: 6573 7202 0000 00da 0f62 6f72 7368 5f63  esr......borsh_c
+00002dd0: 6f6e 7374 7275 6374 727b 0000 00da 1861  onstructr{.....a
+00002de0: 6e63 686f 7270 792e 626f 7273 685f 6578  nchorpy.borsh_ex
+00002df0: 7465 6e73 696f 6e72 0300 0000 da17 616e  tensionr......an
+00002e00: 6368 6f72 7079 2e63 6f64 6572 2e61 6363  chorpy.coder.acc
+00002e10: 6f75 6e74 7372 0400 0000 5a0e 616e 6368  ountsr....Z.anch
+00002e20: 6f72 7079 2e65 7272 6f72 7205 0000 005a  orpy.errorr....Z
+00002e30: 1261 6e63 686f 7270 792e 7574 696c 732e  .anchorpy.utils.
+00002e40: 7270 6372 0600 0000 da14 736f 6c61 6e61  rpcr......solana
+00002e50: 2e72 7063 2e61 7379 6e63 5f61 7069 7207  .rpc.async_apir.
+00002e60: 0000 00da 1573 6f6c 616e 612e 7270 632e  .....solana.rpc.
+00002e70: 636f 6d6d 6974 6d65 6e74 7208 0000 00da  commitmentr.....
+00002e80: 0e73 6f6c 6465 7273 2e70 7562 6b65 7972  .solders.pubkeyr
+00002e90: 0900 0000 da00 720b 0000 0072 4700 0000  ......r....rG...
+00002ea0: 720c 0000 00da 0954 7970 6564 4469 6374  r......TypedDict
+00002eb0: 720d 0000 0072 3f00 0000 723d 0000 0072  r....r?...r=...r
+00002ec0: 3d00 0000 723d 0000 0072 3e00 0000 da08  =...r=...r>.....
+00002ed0: 3c6d 6f64 756c 653e 0100 0000 731c 0000  <module>....s...
+00002ee0: 0008 010c 0208 010c 010c 010c 010c 010c  ................
+00002ef0: 010c 010c 020c 010c 0312 2402 01         ..........$..
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/referral_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/referral_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/referral_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/referral_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/referrer_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/referrer_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/referrer_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/referrer_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/referrer_alias.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/referrer_alias.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/referrer_alias.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/referrer_alias.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/settlement_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/settlement_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/settlement_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/settlement_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/socialized_loss_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/socialized_loss_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/socialized_loss_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/socialized_loss_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/spread_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/spread_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/spread_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/spread_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/state.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/state.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/state.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Sep 12 11:00:06 2023 UTC, .py size: 14179 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b644 0065 6337 0000  a........D.ec7..
+00000000: 610d 0d0a 0000 0000 ae9a 6865 6337 0000  a.........hec7..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a04 6400 6403 6c05  ..d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6400 6407 6c0d  d.l.m.Z...d.d.l.
@@ -102,347 +102,347 @@
 00000650: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
 00000660: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
 00000670: 6d65 5f5f da03 7374 72da 0f5f 5f61 6e6e  me__..str..__ann
 00000680: 6f74 6174 696f 6e73 5f5f da03 696e 74da  otations__..int.
 00000690: 046c 6973 7472 0b00 0000 da0d 6861 6c74  .listr......halt
 000006a0: 5f73 7461 7465 5f76 32da 0f48 616c 7453  _state_v2..HaltS
 000006b0: 7461 7465 5632 4a53 4f4e a900 7239 0000  tateV2JSON..r9..
-000006c0: 0072 3900 0000 fa4b 2f55 7365 7273 2f74  .r9....K/Users/t
+000006c0: 0072 3900 0000 fa59 2f55 7365 7273 2f74  .r9....Y/Users/t
 000006d0: 6672 697a 7a61 2f44 6f63 756d 656e 7473  frizza/Documents
-000006e0: 2f7a 6574 612f 7a65 7461 2d70 792f 7a65  /zeta/zeta-py/ze
-000006f0: 7461 5f70 792f 7a65 7461 5f63 6c69 656e  ta_py/zeta_clien
-00000700: 742f 6163 636f 756e 7473 2f73 7461 7465  t/accounts/state
-00000710: 2e70 7972 0d00 0000 1100 0000 7344 0000  .pyr........sD..
-00000720: 000a 0108 0108 0108 0108 0108 0108 010c  ................
-00000730: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+000006e0: 2f7a 6574 612f 7a65 7461 6d61 726b 6574  /zeta/zetamarket
+000006f0: 732d 7079 2f7a 6574 616d 6172 6b65 7473  s-py/zetamarkets
+00000700: 5f70 792f 7a65 7461 5f63 6c69 656e 742f  _py/zeta_client/
+00000710: 6163 636f 756e 7473 2f73 7461 7465 2e70  accounts/state.p
+00000720: 7972 0d00 0000 1100 0000 7344 0000 000a  yr........sD....
+00000730: 0108 0108 0108 0108 0108 0108 010c 0108  ................
 00000740: 0108 0108 0108 0108 0108 0108 0108 0108  ................
 00000750: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00000760: 0110 0110 0172 0d00 0000 6300 0000 0000  .....r....c.....
-00000770: 0000 0000 0000 0000 0000 0026 0000 0040  ...........&...@
-00000780: 0000 0073 1003 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00000790: 5500 6401 5a03 6504 6a05 6506 6402 3c00  U.d.Z.e.j.e.d.<.
-000007a0: 6507 a008 6403 6509 1b00 6404 6507 6a0a  e...d.e...d.e.j.
-000007b0: 1b00 6405 6507 6a0a 1b00 6406 6507 6a0a  ..d.e.j...d.e.j.
-000007c0: 1b00 6407 6507 6a0a 1b00 6408 6507 6a0a  ..d.e.j...d.e.j.
-000007d0: 1b00 6409 6507 6a0a 640a 1900 1b00 640b  ..d.e.j.d.....d.
-000007e0: 6507 6a0b 1b00 640c 6507 6a0b 1b00 640d  e.j...d.e.j...d.
-000007f0: 6507 6a0b 1b00 640e 6507 6a0b 1b00 640f  e.j...d.e.j...d.
-00000800: 6507 6a0c 1b00 6410 6507 6a0c 1b00 6411  e.j...d.e.j...d.
-00000810: 6507 6a0c 1b00 6412 6507 6a0c 1b00 6413  e.j...d.e.j...d.
-00000820: 6507 6a0b 1b00 6414 6507 6a0a 1b00 6415  e.j...d.e.j...d.
-00000830: 6507 6a0a 1b00 6416 6507 6a0a 1b00 6417  e.j...d.e.j...d.
-00000840: 6507 6a0c 1b00 6418 6507 6a0c 1b00 6419  e.j...d.e.j...d.
-00000850: 6509 1b00 641a 6507 6a0a 1b00 641b 6507  e...d.e.j...d.e.
-00000860: 6a0d 1b00 641c 6509 1b00 641d 6507 6a0a  j...d.e...d.e.j.
-00000870: 1b00 641e 6507 6a0a 1b00 641f 6507 6a0c  ..d.e.j...d.e.j.
-00000880: 1b00 6420 6507 6a0c 1b00 6421 6507 6a0b  ..d e.j...d!e.j.
-00000890: 1b00 6422 6507 6a0c 1b00 6423 650e 6a0f  ..d"e.j...d#e.j.
-000008a0: 6a10 6a11 6424 1900 1b00 6425 650e 6a0f  j.j.d$....d%e.j.
-000008b0: 6a10 6a11 6426 1900 1b00 6427 6507 6a0a  j.j.d&....d'e.j.
-000008c0: 6428 1900 1b00 a122 5a11 6504 6a05 6506  d(....."Z.e.j.e.
-000008d0: 6429 3c00 6512 6506 6403 3c00 6513 6506  d)<.e.e.d.<.e.e.
-000008e0: 6404 3c00 6513 6506 6405 3c00 6513 6506  d.<.e.e.d.<.e.e.
-000008f0: 6406 3c00 6513 6506 6407 3c00 6513 6506  d.<.e.e.d.<.e.e.
-00000900: 6408 3c00 6514 6513 1900 6506 6409 3c00  d.<.e.e...e.d.<.
-00000910: 6513 6506 640b 3c00 6513 6506 640c 3c00  e.e.d.<.e.e.d.<.
-00000920: 6513 6506 640d 3c00 6513 6506 640e 3c00  e.e.d.<.e.e.d.<.
-00000930: 6513 6506 640f 3c00 6513 6506 6410 3c00  e.e.d.<.e.e.d.<.
-00000940: 6513 6506 6411 3c00 6513 6506 6412 3c00  e.e.d.<.e.e.d.<.
-00000950: 6513 6506 6413 3c00 6513 6506 6414 3c00  e.e.d.<.e.e.d.<.
-00000960: 6513 6506 6415 3c00 6513 6506 6416 3c00  e.e.d.<.e.e.d.<.
-00000970: 6513 6506 6417 3c00 6513 6506 6418 3c00  e.e.d.<.e.e.d.<.
-00000980: 6512 6506 6419 3c00 6513 6506 641a 3c00  e.e.d.<.e.e.d.<.
-00000990: 6513 6506 641b 3c00 6512 6506 641c 3c00  e.e.d.<.e.e.d.<.
-000009a0: 6513 6506 641d 3c00 6513 6506 641e 3c00  e.e.d.<.e.e.d.<.
-000009b0: 6513 6506 641f 3c00 6513 6506 6420 3c00  e.e.d.<.e.e.d <.
-000009c0: 6513 6506 6421 3c00 6513 6506 6422 3c00  e.e.d!<.e.e.d"<.
-000009d0: 6514 650e 6a0f 6a10 1900 6506 6423 3c00  e.e.j.j...e.d#<.
-000009e0: 6514 650e 6a0f 6a10 1900 6506 6425 3c00  e.e.j.j...e.d%<.
-000009f0: 6514 6513 1900 6506 6427 3c00 6515 642a  e.e...e.d'<.e.d*
-00000a00: 6516 6602 6517 6512 6504 6a18 6519 1900  e.f.e.e.e.j.e...
-00000a10: 6512 6504 6a18 6400 1900 642b 9c05 642c  e.e.j.d...d+..d,
-00000a20: 642d 8405 8301 5a1a 6515 642a 6516 6602  d-....Z.e.d*e.f.
-00000a30: 6517 6514 6512 1900 6504 6a18 6519 1900  e.e.e...e.j.e...
-00000a40: 6512 6504 6a1b 6504 6a18 6400 1900 1900  e.e.j.e.j.d.....
-00000a50: 642e 9c05 642f 6430 8405 8301 5a1c 6515  d...d/d0....Z.e.
-00000a60: 651d 6400 6431 9c02 6432 6433 8404 8301  e.d.d1..d2d3....
-00000a70: 5a1e 651f 6434 9c01 6435 6436 8404 5a20  Z.e.d4..d5d6..Z 
-00000a80: 6515 651f 6400 6437 9c02 6438 6439 8404  e.e.d.d7..d8d9..
-00000a90: 8301 5a21 642a 5300 293a da05 5374 6174  ..Z!d*S.):..Stat
-00000aa0: 6573 0800 0000 d892 6b5e 684b b6b1 da0d  es......k^hK....
-00000ab0: 6469 7363 7269 6d69 6e61 746f 7272 0e00  discriminatorr..
-00000ac0: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00000ad0: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
-00000ae0: e907 0000 0072 1500 0000 7216 0000 0072  .....r....r....r
-00000af0: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
-00000b00: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
-00000b10: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00000b20: 0072 2100 0000 7222 0000 0072 2300 0000  .r!...r"...r#...
-00000b30: 7224 0000 0072 2500 0000 7226 0000 0072  r$...r%...r&...r
-00000b40: 2700 0000 7228 0000 0072 2900 0000 722a  '...r(...r)...r*
-00000b50: 0000 0072 2b00 0000 722c 0000 0072 2d00  ...r+...r,...r-.
-00000b60: 0000 e905 0000 0072 2e00 0000 e914 0000  .......r........
-00000b70: 0072 2f00 0000 6952 0100 00da 066c 6179  .r/...iR.....lay
-00000b80: 6f75 744e 2905 da04 636f 6e6e da07 6164  outN)...conn..ad
-00000b90: 6472 6573 73da 0a63 6f6d 6d69 746d 656e  dress..commitmen
-00000ba0: 74da 0a70 726f 6772 616d 5f69 64da 0672  t..program_id..r
-00000bb0: 6574 7572 6e63 0500 0000 0000 0000 0000  eturnc..........
-00000bc0: 0000 0800 0000 0400 0000 c300 0000 7348  ..............sH
-00000bd0: 0000 007c 016a 007c 027c 0364 018d 0249  ...|.j.|.|.d...I
-00000be0: 0064 0048 007d 057c 056a 017d 067c 0664  .d.H.}.|.j.}.|.d
-00000bf0: 0075 0072 2664 0053 007c 066a 027c 046b  .u.r&d.S.|.j.|.k
-00000c00: 0372 3874 0364 0283 0182 017c 066a 047d  .r8t.d.....|.j.}
-00000c10: 077c 00a0 057c 07a1 0153 00a9 034e 2901  .|...|...S...N).
-00000c20: 7243 0000 007a 2741 6363 6f75 6e74 2064  rC...z'Account d
-00000c30: 6f65 7320 6e6f 7420 6265 6c6f 6e67 2074  oes not belong t
-00000c40: 6f20 7468 6973 2070 726f 6772 616d 2906  o this program).
-00000c50: da10 6765 745f 6163 636f 756e 745f 696e  ..get_account_in
-00000c60: 666f da05 7661 6c75 65da 056f 776e 6572  fo..value..owner
-00000c70: da0a 5661 6c75 6545 7272 6f72 da04 6461  ..ValueError..da
-00000c80: 7461 da06 6465 636f 6465 2908 da03 636c  ta..decode)...cl
-00000c90: 7372 4100 0000 7242 0000 0072 4300 0000  srA...rB...rC...
-00000ca0: 7244 0000 00da 0472 6573 70da 0469 6e66  rD.....resp..inf
-00000cb0: 6fda 0a62 7974 6573 5f64 6174 6172 3900  o..bytes_datar9.
-00000cc0: 0000 7239 0000 0072 3a00 0000 da05 6665  ..r9...r:.....fe
-00000cd0: 7463 6880 0000 0073 1000 0000 0008 1401  tch....s........
-00000ce0: 0601 0801 0401 0a01 0801 0601 7a0b 5374  ............z.St
-00000cf0: 6174 652e 6665 7463 6829 0572 4100 0000  ate.fetch).rA...
-00000d00: da09 6164 6472 6573 7365 7372 4300 0000  ..addressesrC...
-00000d10: 7244 0000 0072 4500 0000 6305 0000 0000  rD...rE...c.....
-00000d20: 0000 0000 0000 0008 0000 0006 0000 00c3  ................
-00000d30: 0000 0073 6200 0000 7400 7c01 7c02 7c03  ...sb...t.|.|.|.
-00000d40: 6401 8d03 4900 6400 4800 7d05 6700 7d06  d...I.d.H.}.g.}.
-00000d50: 7c05 4400 5d40 7d07 7c07 6400 7500 7234  |.D.]@}.|.d.u.r4
-00000d60: 7c06 a001 6400 a101 0100 711c 7c07 6a02  |...d.....q.|.j.
-00000d70: 6a03 7c04 6b03 7248 7404 6402 8301 8201  j.|.k.rHt.d.....
-00000d80: 7c06 a001 7c00 a005 7c07 6a02 6a06 a101  |...|...|.j.j...
-00000d90: a101 0100 711c 7c06 5300 7246 0000 0029  ....q.|.S.rF...)
-00000da0: 0772 0600 0000 da06 6170 7065 6e64 da07  .r......append..
-00000db0: 6163 636f 756e 7472 4900 0000 724a 0000  accountrI...rJ..
-00000dc0: 0072 4c00 0000 724b 0000 0029 0872 4d00  .rL...rK...).rM.
-00000dd0: 0000 7241 0000 0072 5200 0000 7243 0000  ..rA...rR...rC..
-00000de0: 0072 4400 0000 da05 696e 666f 73da 0372  .rD.....infos..r
-00000df0: 6573 724f 0000 0072 3900 0000 7239 0000  esrO...r9...r9..
-00000e00: 0072 3a00 0000 da0e 6665 7463 685f 6d75  .r:.....fetch_mu
-00000e10: 6c74 6970 6c65 9100 0000 7314 0000 0000  ltiple....s.....
-00000e20: 0814 0104 0108 0108 010a 0102 010c 0108  ................
-00000e30: 0116 017a 1453 7461 7465 2e66 6574 6368  ...z.State.fetch
-00000e40: 5f6d 756c 7469 706c 6529 0272 4b00 0000  _multiple).rK...
-00000e50: 7245 0000 0063 0200 0000 0000 0000 0000  rE...c..........
-00000e60: 0000 0300 0000 2500 0000 4300 0000 73da  ......%...C...s.
-00000e70: 0000 007c 0164 0074 0085 0219 007c 006a  ...|.d.t.....|.j
-00000e80: 016b 0372 1a74 0264 0183 0182 0174 036a  .k.r.t.d.....t.j
-00000e90: 04a0 057c 0174 0064 0085 0219 00a1 017d  ...|.t.d.......}
-00000ea0: 027c 007c 026a 067c 026a 077c 026a 087c  .|.|.j.|.j.|.j.|
-00000eb0: 026a 097c 026a 0a7c 026a 0b7c 026a 0c7c  .j.|.j.|.j.|.j.|
-00000ec0: 026a 0d7c 026a 0e7c 026a 0f7c 026a 107c  .j.|.j.|.j.|.j.|
-00000ed0: 026a 117c 026a 127c 026a 137c 026a 147c  .j.|.j.|.j.|.j.|
-00000ee0: 026a 157c 026a 167c 026a 177c 026a 187c  .j.|.j.|.j.|.j.|
-00000ef0: 026a 197c 026a 1a7c 026a 1b7c 026a 1c7c  .j.|.j.|.j.|.j.|
-00000f00: 026a 1d7c 026a 1e7c 026a 1f7c 026a 207c  .j.|.j.|.j.|.j |
-00000f10: 026a 217c 026a 227c 026a 237c 026a 2474  .j!|.j"|.j#|.j$t
-00000f20: 2574 2664 0264 0384 007c 026a 2783 0283  %t&d.d...|.j'...
-00000f30: 0174 2574 2664 0464 0384 007c 026a 2883  .t%t&d.d...|.j(.
-00000f40: 0283 017c 026a 2964 058d 2253 0029 064e  ...|.j)d.."S.).N
-00000f50: 7a2d 5468 6520 6469 7363 7269 6d69 6e61  z-The discrimina
-00000f60: 746f 7220 666f 7220 7468 6973 2061 6363  tor for this acc
-00000f70: 6f75 6e74 2069 7320 696e 7661 6c69 6463  ount is invalidc
-00000f80: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000f90: 0300 0000 5300 0000 730e 0000 0074 006a  ....S...s....t.j
-00000fa0: 016a 02a0 037c 00a1 0153 00a9 014e a904  .j...|...S...N..
-00000fb0: 720b 0000 0072 3700 0000 da0b 4861 6c74  r....r7.....Halt
-00000fc0: 5374 6174 6556 32da 0c66 726f 6d5f 6465  StateV2..from_de
-00000fd0: 636f 6465 64a9 01da 0469 7465 6d72 3900  coded....itemr9.
-00000fe0: 0000 7239 0000 0072 3a00 0000 da08 3c6c  ..r9...r:.....<l
-00000ff0: 616d 6264 613e cb00 0000 f300 0000 007a  ambda>.........z
-00001000: 1e53 7461 7465 2e64 6563 6f64 652e 3c6c  .State.decode.<l
-00001010: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e63  ocals>.<lambda>c
-00001020: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00001030: 0300 0000 5300 0000 730e 0000 0074 006a  ....S...s....t.j
-00001040: 016a 02a0 037c 00a1 0153 0072 5800 0000  .j...|...S.rX...
-00001050: 7259 0000 0072 5c00 0000 7239 0000 0072  rY...r\...r9...r
-00001060: 3900 0000 723a 0000 0072 5e00 0000 d100  9...r:...r^.....
-00001070: 0000 725f 0000 00a9 2272 0e00 0000 720f  ..r_...."r....r.
-00001080: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
-00001090: 0000 7213 0000 0072 1400 0000 7215 0000  ..r....r....r...
-000010a0: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-000010b0: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-000010c0: 1c00 0000 721d 0000 0072 1e00 0000 721f  ....r....r....r.
-000010d0: 0000 0072 2000 0000 7221 0000 0072 2200  ...r ...r!...r".
-000010e0: 0000 7223 0000 0072 2400 0000 7225 0000  ..r#...r$...r%..
-000010f0: 0072 2600 0000 7227 0000 0072 2800 0000  .r&...r'...r(...
-00001100: 7229 0000 0072 2a00 0000 722b 0000 0072  r)...r*...r+...r
-00001110: 2c00 0000 722d 0000 0072 2e00 0000 722f  ,...r-...r....r/
-00001120: 0000 0029 2a72 0400 0000 723c 0000 0072  ...)*r....r<...r
-00001130: 0500 0000 723b 0000 0072 4000 0000 da05  ....r;...r@.....
-00001140: 7061 7273 6572 0e00 0000 720f 0000 0072  parser....r....r
-00001150: 1000 0000 7211 0000 0072 1200 0000 7213  ....r....r....r.
-00001160: 0000 0072 1400 0000 7215 0000 0072 1600  ...r....r....r..
-00001170: 0000 7217 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00001180: 0072 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00001190: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-000011a0: 2000 0000 7221 0000 0072 2200 0000 7223   ...r!...r"...r#
-000011b0: 0000 0072 2400 0000 7225 0000 0072 2600  ...r$...r%...r&.
-000011c0: 0000 7227 0000 0072 2800 0000 7229 0000  ..r'...r(...r)..
-000011d0: 0072 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
-000011e0: 7236 0000 00da 036d 6170 722d 0000 0072  r6.....mapr-...r
-000011f0: 2e00 0000 722f 0000 0029 0372 4d00 0000  ....r/...).rM...
-00001200: 724b 0000 00da 0364 6563 7239 0000 0072  rK.....decr9...r
-00001210: 3900 0000 723a 0000 0072 4c00 0000 a400  9...r:...rL.....
-00001220: 0000 7362 0000 0000 0212 0108 0114 0102  ..sb............
-00001230: 0104 0104 0104 0104 0104 0104 0104 0104  ................
-00001240: 0104 0104 0104 0104 0104 0104 0104 0104  ................
-00001250: 0104 0104 0104 0104 0104 0104 0104 0104  ................
-00001260: 0104 0104 0104 0104 0104 0104 0104 0102  ................
-00001270: 0102 0106 0104 fe02 ff02 0602 0102 0106  ................
-00001280: 0104 fe02 ff02 0604 d47a 0c53 7461 7465  .........z.State
-00001290: 2e64 6563 6f64 6529 0172 4500 0000 6301  .decode).rE...c.
-000012a0: 0000 0000 0000 0000 0000 0001 0000 0024  ...............$
-000012b0: 0000 0043 0000 0073 b600 0000 7400 7c00  ...C...s....t.|.
-000012c0: 6a01 8301 7c00 6a02 7c00 6a03 7c00 6a04  j...|.j.|.j.|.j.
-000012d0: 7c00 6a05 7c00 6a06 7c00 6a07 7c00 6a08  |.j.|.j.|.j.|.j.
-000012e0: 7c00 6a09 7c00 6a0a 7c00 6a0b 7c00 6a0c  |.j.|.j.|.j.|.j.
-000012f0: 7c00 6a0d 7c00 6a0e 7c00 6a0f 7c00 6a10  |.j.|.j.|.j.|.j.
-00001300: 7c00 6a11 7c00 6a12 7c00 6a13 7c00 6a14  |.j.|.j.|.j.|.j.
-00001310: 7c00 6a15 7400 7c00 6a16 8301 7c00 6a17  |.j.t.|.j...|.j.
-00001320: 7c00 6a18 7400 7c00 6a19 8301 7c00 6a1a  |.j.t.|.j...|.j.
-00001330: 7c00 6a1b 7c00 6a1c 7c00 6a1d 7c00 6a1e  |.j.|.j.|.j.|.j.
-00001340: 7c00 6a1f 7420 7421 6401 6402 8400 7c00  |.j.t t!d.d...|.
-00001350: 6a22 8302 8301 7420 7421 6403 6402 8400  j"....t t!d.d...
-00001360: 7c00 6a23 8302 8301 7c00 6a24 6404 9c22  |.j#....|.j$d.."
-00001370: 5300 2905 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-00001380: 0000 0100 0000 0200 0000 5300 0000 7308  ..........S...s.
-00001390: 0000 007c 00a0 00a1 0053 0072 5800 0000  ...|.....S.rX...
-000013a0: a901 da07 746f 5f6a 736f 6e72 5c00 0000  ....to_jsonr\...
-000013b0: 7239 0000 0072 3900 0000 723a 0000 0072  r9...r9...r:...r
-000013c0: 5e00 0000 f900 0000 725f 0000 007a 1f53  ^.......r_...z.S
-000013d0: 7461 7465 2e74 6f5f 6a73 6f6e 2e3c 6c6f  tate.to_json.<lo
-000013e0: 6361 6c73 3e2e 3c6c 616d 6264 613e 6301  cals>.<lambda>c.
-000013f0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00001400: 0000 0053 0000 0073 0800 0000 7c00 a000  ...S...s....|...
-00001410: a100 5300 7258 0000 0072 6400 0000 725c  ..S.rX...rd...r\
-00001420: 0000 0072 3900 0000 7239 0000 0072 3a00  ...r9...r9...r:.
-00001430: 0000 725e 0000 00fa 0000 0072 5f00 0000  ..r^.......r_...
-00001440: 7260 0000 0029 2572 3300 0000 720e 0000  r`...)%r3...r...
-00001450: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
-00001460: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-00001470: 1500 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
-00001480: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
-00001490: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-000014a0: 0072 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-000014b0: 7222 0000 0072 2300 0000 7224 0000 0072  r"...r#...r$...r
-000014c0: 2500 0000 7226 0000 0072 2700 0000 7228  %...r&...r'...r(
-000014d0: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
-000014e0: 0000 722c 0000 0072 3600 0000 7262 0000  ..r,...r6...rb..
-000014f0: 0072 2d00 0000 722e 0000 0072 2f00 0000  .r-...r....r/...
-00001500: 2901 da04 7365 6c66 7239 0000 0072 3900  )...selfr9...r9.
-00001510: 0000 723a 0000 0072 6500 0000 d800 0000  ..r:...re.......
-00001520: 7346 0000 0000 0208 0104 0104 0104 0104  sF..............
-00001530: 0104 0104 0104 0104 0104 0104 0104 0104  ................
-00001540: 0104 0104 0104 0104 0104 0104 0104 0104  ................
-00001550: 0108 0104 0104 0108 0104 0104 0104 0104  ................
-00001560: 0104 0104 0112 0112 0104 de7a 0d53 7461  ...........z.Sta
-00001570: 7465 2e74 6f5f 6a73 6f6e 2902 da03 6f62  te.to_json)...ob
-00001580: 6a72 4500 0000 6302 0000 0000 0000 0000  jrE...c.........
-00001590: 0000 0002 0000 0026 0000 0043 0000 0073  .......&...C...s
-000015a0: 0201 0000 7c00 7400 a001 7c01 6401 1900  ....|.t...|.d...
-000015b0: a101 7c01 6402 1900 7c01 6403 1900 7c01  ..|.d...|.d...|.
-000015c0: 6404 1900 7c01 6405 1900 7c01 6406 1900  d...|.d...|.d...
-000015d0: 7c01 6407 1900 7c01 6408 1900 7c01 6409  |.d...|.d...|.d.
-000015e0: 1900 7c01 640a 1900 7c01 640b 1900 7c01  ..|.d...|.d...|.
-000015f0: 640c 1900 7c01 640d 1900 7c01 640e 1900  d...|.d...|.d...
-00001600: 7c01 640f 1900 7c01 6410 1900 7c01 6411  |.d...|.d...|.d.
-00001610: 1900 7c01 6412 1900 7c01 6413 1900 7c01  ..|.d...|.d...|.
-00001620: 6414 1900 7c01 6415 1900 7400 a001 7c01  d...|.d...t...|.
-00001630: 6416 1900 a101 7c01 6417 1900 7c01 6418  d.....|.d...|.d.
-00001640: 1900 7400 a001 7c01 6419 1900 a101 7c01  ..t...|.d.....|.
-00001650: 641a 1900 7c01 641b 1900 7c01 641c 1900  d...|.d...|.d...
-00001660: 7c01 641d 1900 7c01 641e 1900 7c01 641f  |.d...|.d...|.d.
-00001670: 1900 7402 7403 6420 6421 8400 7c01 6422  ..t.t.d d!..|.d"
-00001680: 1900 8302 8301 7402 7403 6423 6421 8400  ......t.t.d#d!..
-00001690: 7c01 6424 1900 8302 8301 7c01 6425 1900  |.d$......|.d%..
-000016a0: 6426 8d22 5300 2927 4e72 0e00 0000 720f  d&."S.)'Nr....r.
-000016b0: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
-000016c0: 0000 7213 0000 0072 1400 0000 7215 0000  ..r....r....r...
-000016d0: 0072 1600 0000 7217 0000 0072 1800 0000  .r....r....r....
-000016e0: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-000016f0: 1c00 0000 721d 0000 0072 1e00 0000 721f  ....r....r....r.
-00001700: 0000 0072 2000 0000 7221 0000 0072 2200  ...r ...r!...r".
-00001710: 0000 7223 0000 0072 2400 0000 7225 0000  ..r#...r$...r%..
-00001720: 0072 2600 0000 7227 0000 0072 2800 0000  .r&...r'...r(...
-00001730: 7229 0000 0072 2a00 0000 722b 0000 0072  r)...r*...r+...r
-00001740: 2c00 0000 6301 0000 0000 0000 0000 0000  ,...c...........
-00001750: 0001 0000 0003 0000 0053 0000 0073 0e00  .........S...s..
-00001760: 0000 7400 6a01 6a02 a003 7c00 a101 5300  ..t.j.j...|...S.
-00001770: 7258 0000 00a9 0472 0b00 0000 7237 0000  rX.....r....r7..
-00001780: 0072 5a00 0000 da09 6672 6f6d 5f6a 736f  .rZ.....from_jso
-00001790: 6e72 5c00 0000 7239 0000 0072 3900 0000  nr\...r9...r9...
-000017a0: 723a 0000 0072 5e00 0000 2201 0000 725f  r:...r^..."...r_
-000017b0: 0000 007a 2153 7461 7465 2e66 726f 6d5f  ...z!State.from_
-000017c0: 6a73 6f6e 2e3c 6c6f 6361 6c73 3e2e 3c6c  json.<locals>.<l
-000017d0: 616d 6264 613e 722d 0000 0063 0100 0000  ambda>r-...c....
-000017e0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-000017f0: 5300 0000 730e 0000 0074 006a 016a 02a0  S...s....t.j.j..
-00001800: 037c 00a1 0153 0072 5800 0000 7268 0000  .|...S.rX...rh..
-00001810: 0072 5c00 0000 7239 0000 0072 3900 0000  .r\...r9...r9...
-00001820: 723a 0000 0072 5e00 0000 2801 0000 725f  r:...r^...(...r_
-00001830: 0000 0072 2e00 0000 722f 0000 0072 6000  ...r....r/...r`.
-00001840: 0000 2904 7209 0000 00da 0b66 726f 6d5f  ..).r......from_
-00001850: 7374 7269 6e67 7236 0000 0072 6200 0000  stringr6...rb...
-00001860: 2902 724d 0000 0072 6700 0000 7239 0000  ).rM...rg...r9..
-00001870: 0072 3900 0000 723a 0000 0072 6900 0000  .r9...r:...ri...
-00001880: fe00 0000 735c 0000 0000 0202 010c 0106  ....s\..........
-00001890: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-000018a0: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-000018b0: 0106 0106 0106 010c 0106 0106 010c 0106  ................
-000018c0: 0106 0106 0106 0106 0106 0102 0102 0106  ................
-000018d0: 0106 fe02 ff02 0602 0102 0106 0106 fe02  ................
-000018e0: ff02 0606 d47a 0f53 7461 7465 2e66 726f  .....z.State.fro
-000018f0: 6d5f 6a73 6f6e 2922 7230 0000 0072 3100  m_json)"r0...r1.
-00001900: 0000 7232 0000 0072 3c00 0000 da06 7479  ..r2...r<.....ty
-00001910: 7069 6e67 da08 436c 6173 7356 6172 7234  ping..ClassVarr4
-00001920: 0000 00da 0562 6f72 7368 da07 4353 7472  .....borsh..CStr
-00001930: 7563 7472 0300 0000 da02 5538 da03 5533  uctr......U8..U3
-00001940: 32da 0355 3634 da03 5531 3672 0b00 0000  2..U64..U16r....
-00001950: 7237 0000 0072 5a00 0000 7240 0000 0072  r7...rZ...r@...r
-00001960: 0900 0000 7235 0000 0072 3600 0000 da0b  ....r5...r6.....
-00001970: 636c 6173 736d 6574 686f 6472 0c00 0000  classmethodr....
-00001980: 7207 0000 00da 084f 7074 696f 6e61 6c72  r......Optionalr
-00001990: 0800 0000 7251 0000 00da 044c 6973 7472  ....rQ.....Listr
-000019a0: 5700 0000 da05 6279 7465 7372 4c00 0000  W.....bytesrL...
-000019b0: 720d 0000 0072 6500 0000 7269 0000 0072  r....re...ri...r
-000019c0: 3900 0000 7239 0000 0072 3900 0000 723a  9...r9...r9...r:
-000019d0: 0000 0072 3b00 0000 3600 0000 73c0 0000  ...r;...6...s...
-000019e0: 000a 020e 0104 0106 0108 0108 0108 0108  ................
-000019f0: 0108 010c 0108 0108 0108 0108 0108 0108  ................
-00001a00: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00001a10: 0106 0108 0108 0106 0108 0108 0108 0108  ................
-00001a20: 0108 0108 0110 0110 010c de0e 2408 0108  ............$...
-00001a30: 0108 0108 0108 0108 010c 0108 0108 0108  ................
-00001a40: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00001a50: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00001a60: 0108 0108 0108 0108 0108 0110 0110 010c  ................
-00001a70: 0202 0502 0102 fb02 0202 0102 0108 0102  ................
-00001a80: 0108 fa0e 1002 0502 0102 fb02 0202 0106  ................
-00001a90: 0108 0102 010e fa0e 1202 0112 330e 2602  ............3.&.
-00001aa0: 0172 3b00 0000 291a 726b 0000 00da 0b64  .r;...).rk.....d
-00001ab0: 6174 6163 6c61 7373 6573 7202 0000 00da  ataclassesr.....
-00001ac0: 0f62 6f72 7368 5f63 6f6e 7374 7275 6374  .borsh_construct
-00001ad0: 726d 0000 00da 1861 6e63 686f 7270 792e  rm.....anchorpy.
-00001ae0: 626f 7273 685f 6578 7465 6e73 696f 6e72  borsh_extensionr
-00001af0: 0300 0000 da17 616e 6368 6f72 7079 2e63  ......anchorpy.c
-00001b00: 6f64 6572 2e61 6363 6f75 6e74 7372 0400  oder.accountsr..
-00001b10: 0000 5a0e 616e 6368 6f72 7079 2e65 7272  ..Z.anchorpy.err
-00001b20: 6f72 7205 0000 005a 1261 6e63 686f 7270  orr....Z.anchorp
-00001b30: 792e 7574 696c 732e 7270 6372 0600 0000  y.utils.rpcr....
-00001b40: da14 736f 6c61 6e61 2e72 7063 2e61 7379  ..solana.rpc.asy
-00001b50: 6e63 5f61 7069 7207 0000 00da 1573 6f6c  nc_apir......sol
-00001b60: 616e 612e 7270 632e 636f 6d6d 6974 6d65  ana.rpc.commitme
-00001b70: 6e74 7208 0000 00da 0e73 6f6c 6465 7273  ntr......solders
-00001b80: 2e70 7562 6b65 7972 0900 0000 da00 720b  .pubkeyr......r.
-00001b90: 0000 0072 4400 0000 720c 0000 00da 0954  ...rD...r......T
-00001ba0: 7970 6564 4469 6374 720d 0000 0072 3b00  ypedDictr....r;.
-00001bb0: 0000 7239 0000 0072 3900 0000 7239 0000  ..r9...r9...r9..
-00001bc0: 0072 3a00 0000 da08 3c6d 6f64 756c 653e  .r:.....<module>
-00001bd0: 0100 0000 731c 0000 0008 010c 0208 010c  ....s...........
-00001be0: 010c 010c 010c 010c 010c 010c 020c 010c  ................
-00001bf0: 0312 2502 01                             ..%..
+00000760: 0108 0108 0108 0108 0108 0108 0108 0110  ................
+00000770: 0110 0172 0d00 0000 6300 0000 0000 0000  ...r....c.......
+00000780: 0000 0000 0000 0000 0026 0000 0040 0000  .........&...@..
+00000790: 0073 1003 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
+000007a0: 6401 5a03 6504 6a05 6506 6402 3c00 6507  d.Z.e.j.e.d.<.e.
+000007b0: a008 6403 6509 1b00 6404 6507 6a0a 1b00  ..d.e...d.e.j...
+000007c0: 6405 6507 6a0a 1b00 6406 6507 6a0a 1b00  d.e.j...d.e.j...
+000007d0: 6407 6507 6a0a 1b00 6408 6507 6a0a 1b00  d.e.j...d.e.j...
+000007e0: 6409 6507 6a0a 640a 1900 1b00 640b 6507  d.e.j.d.....d.e.
+000007f0: 6a0b 1b00 640c 6507 6a0b 1b00 640d 6507  j...d.e.j...d.e.
+00000800: 6a0b 1b00 640e 6507 6a0b 1b00 640f 6507  j...d.e.j...d.e.
+00000810: 6a0c 1b00 6410 6507 6a0c 1b00 6411 6507  j...d.e.j...d.e.
+00000820: 6a0c 1b00 6412 6507 6a0c 1b00 6413 6507  j...d.e.j...d.e.
+00000830: 6a0b 1b00 6414 6507 6a0a 1b00 6415 6507  j...d.e.j...d.e.
+00000840: 6a0a 1b00 6416 6507 6a0a 1b00 6417 6507  j...d.e.j...d.e.
+00000850: 6a0c 1b00 6418 6507 6a0c 1b00 6419 6509  j...d.e.j...d.e.
+00000860: 1b00 641a 6507 6a0a 1b00 641b 6507 6a0d  ..d.e.j...d.e.j.
+00000870: 1b00 641c 6509 1b00 641d 6507 6a0a 1b00  ..d.e...d.e.j...
+00000880: 641e 6507 6a0a 1b00 641f 6507 6a0c 1b00  d.e.j...d.e.j...
+00000890: 6420 6507 6a0c 1b00 6421 6507 6a0b 1b00  d e.j...d!e.j...
+000008a0: 6422 6507 6a0c 1b00 6423 650e 6a0f 6a10  d"e.j...d#e.j.j.
+000008b0: 6a11 640a 1900 1b00 6424 650e 6a0f 6a10  j.d.....d$e.j.j.
+000008c0: 6a11 6425 1900 1b00 6426 6507 6a0a 6427  j.d%....d&e.j.d'
+000008d0: 1900 1b00 a122 5a11 6504 6a05 6506 6428  ....."Z.e.j.e.d(
+000008e0: 3c00 6512 6506 6403 3c00 6513 6506 6404  <.e.e.d.<.e.e.d.
+000008f0: 3c00 6513 6506 6405 3c00 6513 6506 6406  <.e.e.d.<.e.e.d.
+00000900: 3c00 6513 6506 6407 3c00 6513 6506 6408  <.e.e.d.<.e.e.d.
+00000910: 3c00 6514 6513 1900 6506 6409 3c00 6513  <.e.e...e.d.<.e.
+00000920: 6506 640b 3c00 6513 6506 640c 3c00 6513  e.d.<.e.e.d.<.e.
+00000930: 6506 640d 3c00 6513 6506 640e 3c00 6513  e.d.<.e.e.d.<.e.
+00000940: 6506 640f 3c00 6513 6506 6410 3c00 6513  e.d.<.e.e.d.<.e.
+00000950: 6506 6411 3c00 6513 6506 6412 3c00 6513  e.d.<.e.e.d.<.e.
+00000960: 6506 6413 3c00 6513 6506 6414 3c00 6513  e.d.<.e.e.d.<.e.
+00000970: 6506 6415 3c00 6513 6506 6416 3c00 6513  e.d.<.e.e.d.<.e.
+00000980: 6506 6417 3c00 6513 6506 6418 3c00 6512  e.d.<.e.e.d.<.e.
+00000990: 6506 6419 3c00 6513 6506 641a 3c00 6513  e.d.<.e.e.d.<.e.
+000009a0: 6506 641b 3c00 6512 6506 641c 3c00 6513  e.d.<.e.e.d.<.e.
+000009b0: 6506 641d 3c00 6513 6506 641e 3c00 6513  e.d.<.e.e.d.<.e.
+000009c0: 6506 641f 3c00 6513 6506 6420 3c00 6513  e.d.<.e.e.d <.e.
+000009d0: 6506 6421 3c00 6513 6506 6422 3c00 6514  e.d!<.e.e.d"<.e.
+000009e0: 650e 6a0f 6a10 1900 6506 6423 3c00 6514  e.j.j...e.d#<.e.
+000009f0: 650e 6a0f 6a10 1900 6506 6424 3c00 6514  e.j.j...e.d$<.e.
+00000a00: 6513 1900 6506 6426 3c00 6515 6429 6516  e...e.d&<.e.d)e.
+00000a10: 6602 6517 6512 6504 6a18 6519 1900 6512  f.e.e.e.j.e...e.
+00000a20: 6504 6a18 6400 1900 642a 9c05 642b 642c  e.j.d...d*..d+d,
+00000a30: 8405 8301 5a1a 6515 6429 6516 6602 6517  ....Z.e.d)e.f.e.
+00000a40: 6514 6512 1900 6504 6a18 6519 1900 6512  e.e...e.j.e...e.
+00000a50: 6504 6a1b 6504 6a18 6400 1900 1900 642d  e.j.e.j.d.....d-
+00000a60: 9c05 642e 642f 8405 8301 5a1c 6515 651d  ..d.d/....Z.e.e.
+00000a70: 6400 6430 9c02 6431 6432 8404 8301 5a1e  d.d0..d1d2....Z.
+00000a80: 651f 6433 9c01 6434 6435 8404 5a20 6515  e.d3..d4d5..Z e.
+00000a90: 651f 6400 6436 9c02 6437 6438 8404 8301  e.d.d6..d7d8....
+00000aa0: 5a21 6429 5300 2939 da05 5374 6174 6573  Z!d)S.)9..States
+00000ab0: 0800 0000 d892 6b5e 684b b6b1 da0d 6469  ......k^hK....di
+00000ac0: 7363 7269 6d69 6e61 746f 7272 0e00 0000  scriminatorr....
+00000ad0: 720f 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
+00000ae0: 1200 0000 7213 0000 0072 1400 0000 e907  ....r....r......
+00000af0: 0000 0072 1500 0000 7216 0000 0072 1700  ...r....r....r..
+00000b00: 0000 7218 0000 0072 1900 0000 721a 0000  ..r....r....r...
+00000b10: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
+00000b20: 721e 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
+00000b30: 2100 0000 7222 0000 0072 2300 0000 7224  !...r"...r#...r$
+00000b40: 0000 0072 2500 0000 7226 0000 0072 2700  ...r%...r&...r'.
+00000b50: 0000 7228 0000 0072 2900 0000 722a 0000  ..r(...r)...r*..
+00000b60: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
+00000b70: 722e 0000 00e9 1200 0000 722f 0000 0069  r.........r/...i
+00000b80: 5201 0000 da06 6c61 796f 7574 4e29 05da  R.....layoutN)..
+00000b90: 0463 6f6e 6eda 0761 6464 7265 7373 da0a  .conn..address..
+00000ba0: 636f 6d6d 6974 6d65 6e74 da0a 7072 6f67  commitment..prog
+00000bb0: 7261 6d5f 6964 da06 7265 7475 726e 6305  ram_id..returnc.
+00000bc0: 0000 0000 0000 0000 0000 0008 0000 0004  ................
+00000bd0: 0000 00c3 0000 0073 4800 0000 7c01 6a00  .......sH...|.j.
+00000be0: 7c02 7c03 6401 8d02 4900 6400 4800 7d05  |.|.d...I.d.H.}.
+00000bf0: 7c05 6a01 7d06 7c06 6400 7500 7226 6400  |.j.}.|.d.u.r&d.
+00000c00: 5300 7c06 6a02 7c04 6b03 7238 7403 6402  S.|.j.|.k.r8t.d.
+00000c10: 8301 8201 7c06 6a04 7d07 7c00 a005 7c07  ....|.j.}.|...|.
+00000c20: a101 5300 a903 4e29 0172 4200 0000 7a27  ..S...N).rB...z'
+00000c30: 4163 636f 756e 7420 646f 6573 206e 6f74  Account does not
+00000c40: 2062 656c 6f6e 6720 746f 2074 6869 7320   belong to this 
+00000c50: 7072 6f67 7261 6d29 06da 1067 6574 5f61  program)...get_a
+00000c60: 6363 6f75 6e74 5f69 6e66 6fda 0576 616c  ccount_info..val
+00000c70: 7565 da05 6f77 6e65 72da 0a56 616c 7565  ue..owner..Value
+00000c80: 4572 726f 72da 0464 6174 61da 0664 6563  Error..data..dec
+00000c90: 6f64 6529 08da 0363 6c73 7240 0000 0072  ode)...clsr@...r
+00000ca0: 4100 0000 7242 0000 0072 4300 0000 da04  A...rB...rC.....
+00000cb0: 7265 7370 da04 696e 666f da0a 6279 7465  resp..info..byte
+00000cc0: 735f 6461 7461 7239 0000 0072 3900 0000  s_datar9...r9...
+00000cd0: 723a 0000 00da 0566 6574 6368 8000 0000  r:.....fetch....
+00000ce0: 7310 0000 0000 0814 0106 0108 0104 010a  s...............
+00000cf0: 0108 0106 017a 0b53 7461 7465 2e66 6574  .....z.State.fet
+00000d00: 6368 2905 7240 0000 00da 0961 6464 7265  ch).r@.....addre
+00000d10: 7373 6573 7242 0000 0072 4300 0000 7244  ssesrB...rC...rD
+00000d20: 0000 0063 0500 0000 0000 0000 0000 0000  ...c............
+00000d30: 0800 0000 0600 0000 c300 0000 7362 0000  ............sb..
+00000d40: 0074 007c 017c 027c 0364 018d 0349 0064  .t.|.|.|.d...I.d
+00000d50: 0048 007d 0567 007d 067c 0544 005d 407d  .H.}.g.}.|.D.]@}
+00000d60: 077c 0764 0075 0072 347c 06a0 0164 00a1  .|.d.u.r4|...d..
+00000d70: 0101 0071 1c7c 076a 026a 037c 046b 0372  ...q.|.j.j.|.k.r
+00000d80: 4874 0464 0283 0182 017c 06a0 017c 00a0  Ht.d.....|...|..
+00000d90: 057c 076a 026a 06a1 01a1 0101 0071 1c7c  .|.j.j.......q.|
+00000da0: 0653 0072 4500 0000 2907 7206 0000 00da  .S.rE...).r.....
+00000db0: 0661 7070 656e 64da 0761 6363 6f75 6e74  .append..account
+00000dc0: 7248 0000 0072 4900 0000 724b 0000 0072  rH...rI...rK...r
+00000dd0: 4a00 0000 2908 724c 0000 0072 4000 0000  J...).rL...r@...
+00000de0: 7251 0000 0072 4200 0000 7243 0000 00da  rQ...rB...rC....
+00000df0: 0569 6e66 6f73 da03 7265 7372 4e00 0000  .infos..resrN...
+00000e00: 7239 0000 0072 3900 0000 723a 0000 00da  r9...r9...r:....
+00000e10: 0e66 6574 6368 5f6d 756c 7469 706c 6591  .fetch_multiple.
+00000e20: 0000 0073 1400 0000 0008 1401 0401 0801  ...s............
+00000e30: 0801 0a01 0201 0c01 0801 1601 7a14 5374  ............z.St
+00000e40: 6174 652e 6665 7463 685f 6d75 6c74 6970  ate.fetch_multip
+00000e50: 6c65 2902 724a 0000 0072 4400 0000 6302  le).rJ...rD...c.
+00000e60: 0000 0000 0000 0000 0000 0003 0000 0025  ...............%
+00000e70: 0000 0043 0000 0073 da00 0000 7c01 6400  ...C...s....|.d.
+00000e80: 7400 8502 1900 7c00 6a01 6b03 721a 7402  t.....|.j.k.r.t.
+00000e90: 6401 8301 8201 7403 6a04 a005 7c01 7400  d.....t.j...|.t.
+00000ea0: 6400 8502 1900 a101 7d02 7c00 7c02 6a06  d.......}.|.|.j.
+00000eb0: 7c02 6a07 7c02 6a08 7c02 6a09 7c02 6a0a  |.j.|.j.|.j.|.j.
+00000ec0: 7c02 6a0b 7c02 6a0c 7c02 6a0d 7c02 6a0e  |.j.|.j.|.j.|.j.
+00000ed0: 7c02 6a0f 7c02 6a10 7c02 6a11 7c02 6a12  |.j.|.j.|.j.|.j.
+00000ee0: 7c02 6a13 7c02 6a14 7c02 6a15 7c02 6a16  |.j.|.j.|.j.|.j.
+00000ef0: 7c02 6a17 7c02 6a18 7c02 6a19 7c02 6a1a  |.j.|.j.|.j.|.j.
+00000f00: 7c02 6a1b 7c02 6a1c 7c02 6a1d 7c02 6a1e  |.j.|.j.|.j.|.j.
+00000f10: 7c02 6a1f 7c02 6a20 7c02 6a21 7c02 6a22  |.j.|.j |.j!|.j"
+00000f20: 7c02 6a23 7c02 6a24 7425 7426 6402 6403  |.j#|.j$t%t&d.d.
+00000f30: 8400 7c02 6a27 8302 8301 7425 7426 6404  ..|.j'....t%t&d.
+00000f40: 6403 8400 7c02 6a28 8302 8301 7c02 6a29  d...|.j(....|.j)
+00000f50: 6405 8d22 5300 2906 4e7a 2d54 6865 2064  d.."S.).Nz-The d
+00000f60: 6973 6372 696d 696e 6174 6f72 2066 6f72  iscriminator for
+00000f70: 2074 6869 7320 6163 636f 756e 7420 6973   this account is
+00000f80: 2069 6e76 616c 6964 6301 0000 0000 0000   invalidc.......
+00000f90: 0000 0000 0001 0000 0003 0000 0053 0000  .............S..
+00000fa0: 0073 0e00 0000 7400 6a01 6a02 a003 7c00  .s....t.j.j...|.
+00000fb0: a101 5300 a901 4ea9 0472 0b00 0000 7237  ..S...N..r....r7
+00000fc0: 0000 00da 0b48 616c 7453 7461 7465 5632  .....HaltStateV2
+00000fd0: da0c 6672 6f6d 5f64 6563 6f64 6564 a901  ..from_decoded..
+00000fe0: da04 6974 656d 7239 0000 0072 3900 0000  ..itemr9...r9...
+00000ff0: 723a 0000 00da 083c 6c61 6d62 6461 3ecb  r:.....<lambda>.
+00001000: 0000 00f3 0000 0000 7a1e 5374 6174 652e  ........z.State.
+00001010: 6465 636f 6465 2e3c 6c6f 6361 6c73 3e2e  decode.<locals>.
+00001020: 3c6c 616d 6264 613e 6301 0000 0000 0000  <lambda>c.......
+00001030: 0000 0000 0001 0000 0003 0000 0053 0000  .............S..
+00001040: 0073 0e00 0000 7400 6a01 6a02 a003 7c00  .s....t.j.j...|.
+00001050: a101 5300 7257 0000 0072 5800 0000 725b  ..S.rW...rX...r[
+00001060: 0000 0072 3900 0000 7239 0000 0072 3a00  ...r9...r9...r:.
+00001070: 0000 725d 0000 00d1 0000 0072 5e00 0000  ..r].......r^...
+00001080: a922 720e 0000 0072 0f00 0000 7210 0000  ."r....r....r...
+00001090: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+000010a0: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+000010b0: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
+000010c0: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
+000010d0: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+000010e0: 0072 2100 0000 7222 0000 0072 2300 0000  .r!...r"...r#...
+000010f0: 7224 0000 0072 2500 0000 7226 0000 0072  r$...r%...r&...r
+00001100: 2700 0000 7228 0000 0072 2900 0000 722a  '...r(...r)...r*
+00001110: 0000 0072 2b00 0000 722c 0000 0072 2d00  ...r+...r,...r-.
+00001120: 0000 722e 0000 0072 2f00 0000 292a 7204  ..r....r/...)*r.
+00001130: 0000 0072 3c00 0000 7205 0000 0072 3b00  ...r<...r....r;.
+00001140: 0000 723f 0000 00da 0570 6172 7365 720e  ..r?.....parser.
+00001150: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
+00001160: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
+00001170: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
+00001180: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00001190: 1b00 0000 721c 0000 0072 1d00 0000 721e  ....r....r....r.
+000011a0: 0000 0072 1f00 0000 7220 0000 0072 2100  ...r....r ...r!.
+000011b0: 0000 7222 0000 0072 2300 0000 7224 0000  ..r"...r#...r$..
+000011c0: 0072 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
+000011d0: 7228 0000 0072 2900 0000 722a 0000 0072  r(...r)...r*...r
+000011e0: 2b00 0000 722c 0000 0072 3600 0000 da03  +...r,...r6.....
+000011f0: 6d61 7072 2d00 0000 722e 0000 0072 2f00  mapr-...r....r/.
+00001200: 0000 2903 724c 0000 0072 4a00 0000 da03  ..).rL...rJ.....
+00001210: 6465 6372 3900 0000 7239 0000 0072 3a00  decr9...r9...r:.
+00001220: 0000 724b 0000 00a4 0000 0073 6200 0000  ..rK.......sb...
+00001230: 0002 1201 0801 1401 0201 0401 0401 0401  ................
+00001240: 0401 0401 0401 0401 0401 0401 0401 0401  ................
+00001250: 0401 0401 0401 0401 0401 0401 0401 0401  ................
+00001260: 0401 0401 0401 0401 0401 0401 0401 0401  ................
+00001270: 0401 0401 0401 0401 0201 0201 0601 04fe  ................
+00001280: 02ff 0206 0201 0201 0601 04fe 02ff 0206  ................
+00001290: 04d4 7a0c 5374 6174 652e 6465 636f 6465  ..z.State.decode
+000012a0: 2901 7244 0000 0063 0100 0000 0000 0000  ).rD...c........
+000012b0: 0000 0000 0100 0000 2400 0000 4300 0000  ........$...C...
+000012c0: 73b6 0000 0074 007c 006a 0183 017c 006a  s....t.|.j...|.j
+000012d0: 027c 006a 037c 006a 047c 006a 057c 006a  .|.j.|.j.|.j.|.j
+000012e0: 067c 006a 077c 006a 087c 006a 097c 006a  .|.j.|.j.|.j.|.j
+000012f0: 0a7c 006a 0b7c 006a 0c7c 006a 0d7c 006a  .|.j.|.j.|.j.|.j
+00001300: 0e7c 006a 0f7c 006a 107c 006a 117c 006a  .|.j.|.j.|.j.|.j
+00001310: 127c 006a 137c 006a 147c 006a 1574 007c  .|.j.|.j.|.j.t.|
+00001320: 006a 1683 017c 006a 177c 006a 1874 007c  .j...|.j.|.j.t.|
+00001330: 006a 1983 017c 006a 1a7c 006a 1b7c 006a  .j...|.j.|.j.|.j
+00001340: 1c7c 006a 1d7c 006a 1e7c 006a 1f74 2074  .|.j.|.j.|.j.t t
+00001350: 2164 0164 0284 007c 006a 2283 0283 0174  !d.d...|.j"....t
+00001360: 2074 2164 0364 0284 007c 006a 2383 0283   t!d.d...|.j#...
+00001370: 017c 006a 2464 049c 2253 0029 054e 6301  .|.j$d.."S.).Nc.
+00001380: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00001390: 0000 0053 0000 0073 0800 0000 7c00 a000  ...S...s....|...
+000013a0: a100 5300 7257 0000 00a9 01da 0774 6f5f  ..S.rW.......to_
+000013b0: 6a73 6f6e 725b 0000 0072 3900 0000 7239  jsonr[...r9...r9
+000013c0: 0000 0072 3a00 0000 725d 0000 00f9 0000  ...r:...r]......
+000013d0: 0072 5e00 0000 7a1f 5374 6174 652e 746f  .r^...z.State.to
+000013e0: 5f6a 736f 6e2e 3c6c 6f63 616c 733e 2e3c  _json.<locals>.<
+000013f0: 6c61 6d62 6461 3e63 0100 0000 0000 0000  lambda>c........
+00001400: 0000 0000 0100 0000 0200 0000 5300 0000  ............S...
+00001410: 7308 0000 007c 00a0 00a1 0053 0072 5700  s....|.....S.rW.
+00001420: 0000 7263 0000 0072 5b00 0000 7239 0000  ..rc...r[...r9..
+00001430: 0072 3900 0000 723a 0000 0072 5d00 0000  .r9...r:...r]...
+00001440: fa00 0000 725e 0000 0072 5f00 0000 2925  ....r^...r_...)%
+00001450: 7233 0000 0072 0e00 0000 720f 0000 0072  r3...r....r....r
+00001460: 1000 0000 7211 0000 0072 1200 0000 7213  ....r....r....r.
+00001470: 0000 0072 1400 0000 7215 0000 0072 1600  ...r....r....r..
+00001480: 0000 7217 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00001490: 0072 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
+000014a0: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+000014b0: 2000 0000 7221 0000 0072 2200 0000 7223   ...r!...r"...r#
+000014c0: 0000 0072 2400 0000 7225 0000 0072 2600  ...r$...r%...r&.
+000014d0: 0000 7227 0000 0072 2800 0000 7229 0000  ..r'...r(...r)..
+000014e0: 0072 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
+000014f0: 7236 0000 0072 6100 0000 722d 0000 0072  r6...ra...r-...r
+00001500: 2e00 0000 722f 0000 0029 01da 0473 656c  ....r/...)...sel
+00001510: 6672 3900 0000 7239 0000 0072 3a00 0000  fr9...r9...r:...
+00001520: 7264 0000 00d8 0000 0073 4600 0000 0002  rd.......sF.....
+00001530: 0801 0401 0401 0401 0401 0401 0401 0401  ................
+00001540: 0401 0401 0401 0401 0401 0401 0401 0401  ................
+00001550: 0401 0401 0401 0401 0401 0801 0401 0401  ................
+00001560: 0801 0401 0401 0401 0401 0401 0401 1201  ................
+00001570: 1201 04de 7a0d 5374 6174 652e 746f 5f6a  ....z.State.to_j
+00001580: 736f 6e29 02da 036f 626a 7244 0000 0063  son)...objrD...c
+00001590: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000015a0: 2600 0000 4300 0000 7302 0100 007c 0074  &...C...s....|.t
+000015b0: 00a0 017c 0164 0119 00a1 017c 0164 0219  ...|.d.....|.d..
+000015c0: 007c 0164 0319 007c 0164 0419 007c 0164  .|.d...|.d...|.d
+000015d0: 0519 007c 0164 0619 007c 0164 0719 007c  ...|.d...|.d...|
+000015e0: 0164 0819 007c 0164 0919 007c 0164 0a19  .d...|.d...|.d..
+000015f0: 007c 0164 0b19 007c 0164 0c19 007c 0164  .|.d...|.d...|.d
+00001600: 0d19 007c 0164 0e19 007c 0164 0f19 007c  ...|.d...|.d...|
+00001610: 0164 1019 007c 0164 1119 007c 0164 1219  .d...|.d...|.d..
+00001620: 007c 0164 1319 007c 0164 1419 007c 0164  .|.d...|.d...|.d
+00001630: 1519 0074 00a0 017c 0164 1619 00a1 017c  ...t...|.d.....|
+00001640: 0164 1719 007c 0164 1819 0074 00a0 017c  .d...|.d...t...|
+00001650: 0164 1919 00a1 017c 0164 1a19 007c 0164  .d.....|.d...|.d
+00001660: 1b19 007c 0164 1c19 007c 0164 1d19 007c  ...|.d...|.d...|
+00001670: 0164 1e19 007c 0164 1f19 0074 0274 0364  .d...|.d...t.t.d
+00001680: 2064 2184 007c 0164 2219 0083 0283 0174   d!..|.d"......t
+00001690: 0274 0364 2364 2184 007c 0164 2419 0083  .t.d#d!..|.d$...
+000016a0: 0283 017c 0164 2519 0064 268d 2253 0029  ...|.d%..d&."S.)
+000016b0: 274e 720e 0000 0072 0f00 0000 7210 0000  'Nr....r....r...
+000016c0: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+000016d0: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+000016e0: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
+000016f0: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
+00001700: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+00001710: 0072 2100 0000 7222 0000 0072 2300 0000  .r!...r"...r#...
+00001720: 7224 0000 0072 2500 0000 7226 0000 0072  r$...r%...r&...r
+00001730: 2700 0000 7228 0000 0072 2900 0000 722a  '...r(...r)...r*
+00001740: 0000 0072 2b00 0000 722c 0000 0063 0100  ...r+...r,...c..
+00001750: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00001760: 0000 5300 0000 730e 0000 0074 006a 016a  ..S...s....t.j.j
+00001770: 02a0 037c 00a1 0153 0072 5700 0000 a904  ...|...S.rW.....
+00001780: 720b 0000 0072 3700 0000 7259 0000 00da  r....r7...rY....
+00001790: 0966 726f 6d5f 6a73 6f6e 725b 0000 0072  .from_jsonr[...r
+000017a0: 3900 0000 7239 0000 0072 3a00 0000 725d  9...r9...r:...r]
+000017b0: 0000 0022 0100 0072 5e00 0000 7a21 5374  ..."...r^...z!St
+000017c0: 6174 652e 6672 6f6d 5f6a 736f 6e2e 3c6c  ate.from_json.<l
+000017d0: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e72  ocals>.<lambda>r
+000017e0: 2d00 0000 6301 0000 0000 0000 0000 0000  -...c...........
+000017f0: 0001 0000 0003 0000 0053 0000 0073 0e00  .........S...s..
+00001800: 0000 7400 6a01 6a02 a003 7c00 a101 5300  ..t.j.j...|...S.
+00001810: 7257 0000 0072 6700 0000 725b 0000 0072  rW...rg...r[...r
+00001820: 3900 0000 7239 0000 0072 3a00 0000 725d  9...r9...r:...r]
+00001830: 0000 0028 0100 0072 5e00 0000 722e 0000  ...(...r^...r...
+00001840: 0072 2f00 0000 725f 0000 0029 0472 0900  .r/...r_...).r..
+00001850: 0000 da0b 6672 6f6d 5f73 7472 696e 6772  ....from_stringr
+00001860: 3600 0000 7261 0000 0029 0272 4c00 0000  6...ra...).rL...
+00001870: 7266 0000 0072 3900 0000 7239 0000 0072  rf...r9...r9...r
+00001880: 3a00 0000 7268 0000 00fe 0000 0073 5c00  :...rh.......s\.
+00001890: 0000 0002 0201 0c01 0601 0601 0601 0601  ................
+000018a0: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+000018b0: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+000018c0: 0c01 0601 0601 0c01 0601 0601 0601 0601  ................
+000018d0: 0601 0601 0201 0201 0601 06fe 02ff 0206  ................
+000018e0: 0201 0201 0601 06fe 02ff 0206 06d4 7a0f  ..............z.
+000018f0: 5374 6174 652e 6672 6f6d 5f6a 736f 6e29  State.from_json)
+00001900: 2272 3000 0000 7231 0000 0072 3200 0000  "r0...r1...r2...
+00001910: 723c 0000 00da 0674 7970 696e 67da 0843  r<.....typing..C
+00001920: 6c61 7373 5661 7272 3400 0000 da05 626f  lassVarr4.....bo
+00001930: 7273 68da 0743 5374 7275 6374 7203 0000  rsh..CStructr...
+00001940: 00da 0255 38da 0355 3332 da03 5536 34da  ...U8..U32..U64.
+00001950: 0355 3136 720b 0000 0072 3700 0000 7259  .U16r....r7...rY
+00001960: 0000 0072 3f00 0000 7209 0000 0072 3500  ...r?...r....r5.
+00001970: 0000 7236 0000 00da 0b63 6c61 7373 6d65  ..r6.....classme
+00001980: 7468 6f64 720c 0000 0072 0700 0000 da08  thodr....r......
+00001990: 4f70 7469 6f6e 616c 7208 0000 0072 5000  Optionalr....rP.
+000019a0: 0000 da04 4c69 7374 7256 0000 00da 0562  ....ListrV.....b
+000019b0: 7974 6573 724b 0000 0072 0d00 0000 7264  ytesrK...r....rd
+000019c0: 0000 0072 6800 0000 7239 0000 0072 3900  ...rh...r9...r9.
+000019d0: 0000 7239 0000 0072 3a00 0000 723b 0000  ..r9...r:...r;..
+000019e0: 0036 0000 0073 c000 0000 0a02 0e01 0401  .6...s..........
+000019f0: 0601 0801 0801 0801 0801 0801 0c01 0801  ................
+00001a00: 0801 0801 0801 0801 0801 0801 0801 0801  ................
+00001a10: 0801 0801 0801 0801 0801 0601 0801 0801  ................
+00001a20: 0601 0801 0801 0801 0801 0801 0801 1001  ................
+00001a30: 1001 0cde 0e24 0801 0801 0801 0801 0801  .....$..........
+00001a40: 0801 0c01 0801 0801 0801 0801 0801 0801  ................
+00001a50: 0801 0801 0801 0801 0801 0801 0801 0801  ................
+00001a60: 0801 0801 0801 0801 0801 0801 0801 0801  ................
+00001a70: 0801 0801 1001 1001 0c02 0205 0201 02fb  ................
+00001a80: 0202 0201 0201 0801 0201 08fa 0e10 0205  ................
+00001a90: 0201 02fb 0202 0201 0601 0801 0201 0efa  ................
+00001aa0: 0e12 0201 1233 0e26 0201 723b 0000 0029  .....3.&..r;...)
+00001ab0: 1a72 6a00 0000 da0b 6461 7461 636c 6173  .rj.....dataclas
+00001ac0: 7365 7372 0200 0000 da0f 626f 7273 685f  sesr......borsh_
+00001ad0: 636f 6e73 7472 7563 7472 6c00 0000 da18  constructrl.....
+00001ae0: 616e 6368 6f72 7079 2e62 6f72 7368 5f65  anchorpy.borsh_e
+00001af0: 7874 656e 7369 6f6e 7203 0000 00da 1761  xtensionr......a
+00001b00: 6e63 686f 7270 792e 636f 6465 722e 6163  nchorpy.coder.ac
+00001b10: 636f 756e 7473 7204 0000 005a 0e61 6e63  countsr....Z.anc
+00001b20: 686f 7270 792e 6572 726f 7272 0500 0000  horpy.errorr....
+00001b30: 5a12 616e 6368 6f72 7079 2e75 7469 6c73  Z.anchorpy.utils
+00001b40: 2e72 7063 7206 0000 00da 1473 6f6c 616e  .rpcr......solan
+00001b50: 612e 7270 632e 6173 796e 635f 6170 6972  a.rpc.async_apir
+00001b60: 0700 0000 da15 736f 6c61 6e61 2e72 7063  ......solana.rpc
+00001b70: 2e63 6f6d 6d69 746d 656e 7472 0800 0000  .commitmentr....
+00001b80: da0e 736f 6c64 6572 732e 7075 626b 6579  ..solders.pubkey
+00001b90: 7209 0000 00da 0072 0b00 0000 7243 0000  r......r....rC..
+00001ba0: 0072 0c00 0000 da09 5479 7065 6444 6963  .r......TypedDic
+00001bb0: 7472 0d00 0000 723b 0000 0072 3900 0000  tr....r;...r9...
+00001bc0: 7239 0000 0072 3900 0000 723a 0000 00da  r9...r9...r:....
+00001bd0: 083c 6d6f 6475 6c65 3e01 0000 0073 1c00  .<module>....s..
+00001be0: 0000 0801 0c02 0801 0c01 0c01 0c01 0c01  ................
+00001bf0: 0c01 0c01 0c02 0c01 0c03 1225 0201       ...........%..
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/underlying.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/underlying.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/underlying.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/underlying.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_deposit_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_deposit_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_deposit_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_deposit_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_insurance_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_insurance_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_insurance_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_insurance_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_trading_fees_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_trading_fees_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_trading_fees_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/whitelist_trading_fees_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/zeta_group.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/zeta_group.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/__pycache__/zeta_group.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/__pycache__/zeta_group.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/cross_margin_account.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/cross_margin_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,21 @@
         "authority" / BorshPubkey,
         "delegated_pubkey" / BorshPubkey,
         "balance" / borsh.U64,
         "subaccount_index" / borsh.U8,
         "nonce" / borsh.U8,
         "force_cancel_flag" / borsh.Bool,
         "account_type" / types.margin_account_type.layout,
-        "open_orders_nonces" / borsh.U8[5],
-        "open_orders_nonces_padding" / borsh.U8[20],
+        "open_orders_nonces" / borsh.U8[7],
+        "open_orders_nonces_padding" / borsh.U8[18],
         "rebalance_amount" / borsh.I64,
-        "last_funding_deltas" / types.anchor_decimal.AnchorDecimal.layout[5],
-        "last_funding_deltas_padding" / types.anchor_decimal.AnchorDecimal.layout[20],
-        "product_ledgers" / types.product_ledger.ProductLedger.layout[5],
-        "product_ledgers_padding" / types.product_ledger.ProductLedger.layout[20],
+        "last_funding_deltas" / types.anchor_decimal.AnchorDecimal.layout[7],
+        "last_funding_deltas_padding" / types.anchor_decimal.AnchorDecimal.layout[18],
+        "product_ledgers" / types.product_ledger.ProductLedger.layout[7],
+        "product_ledgers_padding" / types.product_ledger.ProductLedger.layout[18],
         "padding" / borsh.U8[2000],
     )
     authority: Pubkey
     delegated_pubkey: Pubkey
     balance: int
     subaccount_index: int
     nonce: int
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/pricing.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/pricing.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,45 +51,45 @@
 
 
 @dataclass
 class Pricing:
     discriminator: typing.ClassVar = b"\xbe{\xd2\xb6\x8f\x0b\x98\x88"
     layout: typing.ClassVar = borsh.CStruct(
         "nonce" / borsh.U8,
-        "mark_prices" / borsh.U64[5],
-        "mark_prices_padding" / borsh.U64[20],
-        "update_timestamps" / borsh.U64[5],
-        "update_timestamps_padding" / borsh.U64[20],
-        "funding_deltas" / types.anchor_decimal.AnchorDecimal.layout[5],
-        "funding_deltas_padding" / types.anchor_decimal.AnchorDecimal.layout[20],
-        "latest_funding_rates" / types.anchor_decimal.AnchorDecimal.layout[5],
-        "latest_funding_rates_padding" / types.anchor_decimal.AnchorDecimal.layout[20],
-        "latest_midpoints" / borsh.U64[5],
-        "latest_midpoints_padding" / borsh.U64[20],
-        "oracles" / BorshPubkey[5],
-        "oracles_padding" / BorshPubkey[20],
-        "oracle_backup_feeds" / BorshPubkey[5],
-        "oracle_backup_feeds_padding" / BorshPubkey[20],
-        "markets" / BorshPubkey[5],
-        "markets_padding" / BorshPubkey[20],
-        "perp_sync_queues" / BorshPubkey[5],
-        "perp_sync_queues_padding" / BorshPubkey[20],
-        "perp_parameters" / types.perp_parameters.PerpParameters.layout[5],
-        "perp_parameters_padding" / types.perp_parameters.PerpParameters.layout[20],
-        "margin_parameters" / types.margin_parameters.MarginParameters.layout[5],
-        "margin_parameters_padding" / types.margin_parameters.MarginParameters.layout[20],
-        "products" / types.product.Product.layout[5],
-        "products_padding" / types.product.Product.layout[20],
-        "zeta_group_keys" / BorshPubkey[5],
-        "zeta_group_keys_padding" / BorshPubkey[20],
+        "mark_prices" / borsh.U64[7],
+        "mark_prices_padding" / borsh.U64[18],
+        "update_timestamps" / borsh.U64[7],
+        "update_timestamps_padding" / borsh.U64[18],
+        "funding_deltas" / types.anchor_decimal.AnchorDecimal.layout[7],
+        "funding_deltas_padding" / types.anchor_decimal.AnchorDecimal.layout[18],
+        "latest_funding_rates" / types.anchor_decimal.AnchorDecimal.layout[7],
+        "latest_funding_rates_padding" / types.anchor_decimal.AnchorDecimal.layout[18],
+        "latest_midpoints" / borsh.U64[7],
+        "latest_midpoints_padding" / borsh.U64[18],
+        "oracles" / BorshPubkey[7],
+        "oracles_padding" / BorshPubkey[18],
+        "oracle_backup_feeds" / BorshPubkey[7],
+        "oracle_backup_feeds_padding" / BorshPubkey[18],
+        "markets" / BorshPubkey[7],
+        "markets_padding" / BorshPubkey[18],
+        "perp_sync_queues" / BorshPubkey[7],
+        "perp_sync_queues_padding" / BorshPubkey[18],
+        "perp_parameters" / types.perp_parameters.PerpParameters.layout[7],
+        "perp_parameters_padding" / types.perp_parameters.PerpParameters.layout[18],
+        "margin_parameters" / types.margin_parameters.MarginParameters.layout[7],
+        "margin_parameters_padding" / types.margin_parameters.MarginParameters.layout[18],
+        "products" / types.product.Product.layout[7],
+        "products_padding" / types.product.Product.layout[18],
+        "zeta_group_keys" / BorshPubkey[7],
+        "zeta_group_keys_padding" / BorshPubkey[18],
         "total_insurance_vault_deposits" / borsh.U64,
         "last_withdraw_timestamp" / borsh.U64,
         "net_outflow_sum" / borsh.I64,
-        "halt_force_pricing" / borsh.Bool[5],
-        "halt_force_pricing_padding" / borsh.Bool[20],
+        "halt_force_pricing" / borsh.Bool[7],
+        "halt_force_pricing_padding" / borsh.Bool[18],
         "padding" / borsh.U8[2707],
     )
     nonce: int
     mark_prices: list[int]
     mark_prices_padding: list[int]
     update_timestamps: list[int]
     update_timestamps_padding: list[int]
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/accounts/state.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/accounts/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,16 +82,16 @@
         "secondary_admin" / BorshPubkey,
         "vault_nonce" / borsh.U8,
         "insurance_vault_nonce" / borsh.U8,
         "deprecated_total_insurance_vault_deposits" / borsh.U64,
         "native_withdraw_limit" / borsh.U64,
         "withdraw_limit_epoch_seconds" / borsh.U32,
         "native_open_interest_limit" / borsh.U64,
-        "halt_states" / types.halt_state_v2.HaltStateV2.layout[5],
-        "halt_states_padding" / types.halt_state_v2.HaltStateV2.layout[20],
+        "halt_states" / types.halt_state_v2.HaltStateV2.layout[7],
+        "halt_states_padding" / types.halt_state_v2.HaltStateV2.layout[18],
         "padding" / borsh.U8[338],
     )
     admin: Pubkey
     state_nonce: int
     serum_nonce: int
     mint_auth_nonce: int
     num_underlyings: int
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/__init__.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/__pycache__/__init__.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/__pycache__/__init__.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/__pycache__/anchor.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/__pycache__/anchor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/__pycache__/anchor.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/__pycache__/anchor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/__pycache__/custom.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/__pycache__/custom.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/__pycache__/custom.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/__pycache__/custom.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/anchor.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/anchor.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/errors/custom.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/errors/custom.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__init__.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/__init__.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/__init__.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/add_market_indexes.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/add_market_indexes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/add_market_indexes.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/add_market_indexes.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/add_perp_market_index.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/add_perp_market_index.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/add_perp_market_index.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/add_perp_market_index.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/apply_perp_funding.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/apply_perp_funding.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/apply_perp_funding.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/apply_perp_funding.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/burn_vault_tokens.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/burn_vault_tokens.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/burn_vault_tokens.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/burn_vault_tokens.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_all_market_orders.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_all_market_orders.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_all_market_orders.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_all_market_orders.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_by_client_order_id.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_by_client_order_id.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_by_client_order_id.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_by_client_order_id.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_by_client_order_id_no_error.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_by_client_order_id_no_error.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_by_client_order_id_no_error.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_by_client_order_id_no_error.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_halted.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_halted.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_halted.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_halted.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_no_error.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_no_error.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_no_error.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/cancel_order_no_error.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/claim_referrals_rewards.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/claim_referrals_rewards.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/claim_referrals_rewards.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/claim_referrals_rewards.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/clean_zeta_market_halted.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/clean_zeta_market_halted.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/clean_zeta_market_halted.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/clean_zeta_market_halted.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/clean_zeta_markets.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/clean_zeta_markets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/clean_zeta_markets.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/clean_zeta_markets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_cross_margin_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_cross_margin_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_cross_margin_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_cross_margin_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_cross_margin_account_manager.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_cross_margin_account_manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_cross_margin_account_manager.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_cross_margin_account_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_margin_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_margin_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_margin_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_margin_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders_v2.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders_v2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders_v2.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders_v2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders_v3.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders_v3.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders_v3.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_open_orders_v3.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_spread_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_spread_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/close_spread_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/close_spread_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/collect_treasury_funds.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/collect_treasury_funds.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/collect_treasury_funds.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/collect_treasury_funds.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/crank_event_queue.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/crank_event_queue.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/crank_event_queue.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/crank_event_queue.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/deposit.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/deposit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/deposit.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/deposit.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_insurance_vault.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_insurance_vault.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_insurance_vault.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_insurance_vault.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_insurance_vault_v2.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_insurance_vault_v2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_insurance_vault_v2.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_insurance_vault_v2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_v2.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_v2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_v2.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/deposit_v2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/edit_delegated_pubkey.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/edit_delegated_pubkey.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/edit_delegated_pubkey.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/edit_delegated_pubkey.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/expire_series.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/expire_series.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/expire_series.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/expire_series.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/expire_series_override.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/expire_series_override.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/expire_series_override.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/expire_series_override.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_order_by_order_id.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_order_by_order_id.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_order_by_order_id.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_order_by_order_id.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_order_by_order_id_v2.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_order_by_order_id_v2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_order_by_order_id_v2.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_order_by_order_id_v2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_orders.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_orders.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_orders.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_orders.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_orders_v2.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_orders_v2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_orders_v2.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/force_cancel_orders_v2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/halt.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/halt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/halt.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/halt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_insurance_vault.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_insurance_vault.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_insurance_vault.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_insurance_vault.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_socialized_loss_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_socialized_loss_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_socialized_loss_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_socialized_loss_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_vault.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_vault.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_vault.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_combined_vault.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_cross_margin_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_cross_margin_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_cross_margin_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_cross_margin_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_cross_margin_account_manager.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_cross_margin_account_manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_cross_margin_account_manager.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_cross_margin_account_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_insurance_deposit_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_insurance_deposit_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_insurance_deposit_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_insurance_deposit_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_margin_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_margin_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_margin_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_margin_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_indexes.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_indexes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_indexes.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_indexes.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_node.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_node.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_node.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_node.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_strikes.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_strikes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_strikes.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_strikes.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_tif_epoch_cycle.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_tif_epoch_cycle.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_tif_epoch_cycle.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_market_tif_epoch_cycle.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders_v2.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders_v2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders_v2.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders_v2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders_v3.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders_v3.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders_v3.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_open_orders_v3.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_perp_sync_queue.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_perp_sync_queue.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_perp_sync_queue.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_perp_sync_queue.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_referrer_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_referrer_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_referrer_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_referrer_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_referrer_alias.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_referrer_alias.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_referrer_alias.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_referrer_alias.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_spread_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_spread_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_spread_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_spread_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_underlying.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_underlying.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_underlying.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_underlying.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_deposit_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_deposit_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_deposit_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_deposit_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_insurance_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_insurance_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_insurance_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_insurance_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_trading_fees_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_trading_fees_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_trading_fees_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_whitelist_trading_fees_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_group.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_group.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_group.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_group.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_market.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_market.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_market.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_market.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_pricing.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_pricing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_pricing.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_pricing.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_referrals_rewards_wallet.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_referrals_rewards_wallet.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_referrals_rewards_wallet.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_referrals_rewards_wallet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_state.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_state.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_treasury_wallet.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_treasury_wallet.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_treasury_wallet.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/initialize_zeta_treasury_wallet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/liquidate.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/liquidate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/liquidate.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/liquidate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/liquidate_v2.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/liquidate_v2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/liquidate_v2.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/liquidate_v2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/migrate_to_cross_margin_account.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/migrate_to_cross_margin_account.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/migrate_to_cross_margin_account.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/migrate_to_cross_margin_account.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/override_expiry.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/override_expiry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/override_expiry.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/override_expiry.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_order.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_order.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_order.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_order.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v2.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v2.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v3.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v3.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v3.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v3.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v4.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v4.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v4.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_order_v4.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order_v2.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order_v2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order_v2.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order_v2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order_v3.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order_v3.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order_v3.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/place_perp_order_v3.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/position_movement.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/position_movement.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/position_movement.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/position_movement.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/prune_expired_tif_orders.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/prune_expired_tif_orders.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/prune_expired_tif_orders.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/prune_expired_tif_orders.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/rebalance_insurance_vault.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/rebalance_insurance_vault.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/rebalance_insurance_vault.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/rebalance_insurance_vault.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/refer_user.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/refer_user.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/refer_user.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/refer_user.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/reset_num_flex_underlyings.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/reset_num_flex_underlyings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/reset_num_flex_underlyings.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/reset_num_flex_underlyings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/set_referrals_rewards.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/set_referrals_rewards.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/set_referrals_rewards.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/set_referrals_rewards.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/settle_dex_funds.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/settle_dex_funds.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/settle_dex_funds.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/settle_dex_funds.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/settle_positions_halted.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/settle_positions_halted.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/settle_positions_halted.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/settle_positions_halted.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/toggle_market_maker.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/toggle_market_maker.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/toggle_market_maker.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/toggle_market_maker.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/toggle_zeta_group_perps_only.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/toggle_zeta_group_perps_only.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/toggle_zeta_group_perps_only.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/toggle_zeta_group_perps_only.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/transfer_excess_spread_balance.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/transfer_excess_spread_balance.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/transfer_excess_spread_balance.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/transfer_excess_spread_balance.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/treasury_movement.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/treasury_movement.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/treasury_movement.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/treasury_movement.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/unhalt.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/unhalt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/unhalt.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/unhalt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_admin.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_admin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_admin.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_admin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_halt_state.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_halt_state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_halt_state.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_halt_state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_interest_rate.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_interest_rate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_interest_rate.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_interest_rate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_margin_parameters.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_margin_parameters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_margin_parameters.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_margin_parameters.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_oracle.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_oracle.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_oracle.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_oracle.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_oracle_backup_feed.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_oracle_backup_feed.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_oracle_backup_feed.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_oracle_backup_feed.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_perp_parameters.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_perp_parameters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_perp_parameters.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_perp_parameters.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_pricing_parameters.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_pricing_parameters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_pricing_parameters.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_pricing_parameters.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_pricing_v2.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_pricing_v2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_pricing_v2.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_pricing_v2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_referrals_admin.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_referrals_admin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_referrals_admin.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_referrals_admin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_secondary_admin.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_secondary_admin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_secondary_admin.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_secondary_admin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_volatility.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_volatility.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_volatility.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_volatility.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_expiry_parameters.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_expiry_parameters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_expiry_parameters.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_expiry_parameters.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_margin_parameters.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_margin_parameters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_margin_parameters.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_margin_parameters.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_perp_parameters.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_perp_parameters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_perp_parameters.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_group_perp_parameters.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_pricing_pubkeys.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_pricing_pubkeys.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_pricing_pubkeys.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_pricing_pubkeys.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_state.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_state.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/update_zeta_state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_insurance_vault.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_insurance_vault.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_insurance_vault.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_insurance_vault.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_insurance_vault_v2.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_insurance_vault_v2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_insurance_vault_v2.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_insurance_vault_v2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_v2.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_v2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_v2.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/__pycache__/withdraw_v2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/apply_perp_funding.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/apply_perp_funding.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/cancel_all_market_orders.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/cancel_all_market_orders.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/cancel_order.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/cancel_order.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/cancel_order_by_client_order_id.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/cancel_order_by_client_order_id.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/cancel_order_by_client_order_id_no_error.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/cancel_order_by_client_order_id_no_error.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/cancel_order_halted.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/cancel_order_halted.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/cancel_order_no_error.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/cancel_order_no_error.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/claim_referrals_rewards.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/claim_referrals_rewards.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/close_cross_margin_account.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/close_cross_margin_account.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/close_cross_margin_account_manager.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/close_cross_margin_account_manager.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/close_open_orders_v3.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/close_open_orders_v3.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/crank_event_queue.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/crank_event_queue.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/deposit_v2.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/deposit_v2.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/initialize_cross_margin_account.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/initialize_cross_margin_account.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/initialize_cross_margin_account_manager.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/initialize_cross_margin_account_manager.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/initialize_open_orders_v3.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/initialize_open_orders_v3.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/initialize_referrer_account.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/initialize_referrer_account.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/initialize_referrer_alias.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/initialize_referrer_alias.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/initialize_zeta_referrals_rewards_wallet.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/initialize_zeta_referrals_rewards_wallet.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/liquidate_v2.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/liquidate_v2.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/place_perp_order_v3.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/place_perp_order_v3.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/place_perp_order_v4.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/place_perp_order_v4.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/refer_user.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/refer_user.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/instructions/withdraw_v2.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/instructions/withdraw_v2.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__init__.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,134 +1,102 @@
 import typing
 
 from . import (
     anchor_decimal,
     asset,
     cross_margin_account_info,
-    expire_series_override_args,
-    expiry_series,
-    expiry_series_status,
     halt_args,
     halt_state,
     halt_state_args,
     halt_state_v2,
     initialize_market_args,
     initialize_market_node_args,
     initialize_state_args,
-    initialize_zeta_group_args,
     initialize_zeta_pricing_args,
     kind,
     margin_account_type,
     margin_parameters,
     margin_requirement,
     movement_type,
     order_complete_type,
     order_state,
     order_type,
-    override_expiry_args,
     perp_parameters,
     place_order_type,
     position,
-    position_movement_arg,
     pricing_parameters,
     product,
     product_greeks,
     product_ledger,
     set_referrals_rewards_args,
     side,
     strike,
     trait_type,
     treasury_movement_type,
-    update_greeks_args,
-    update_interest_rate_args,
     update_margin_parameters_args,
     update_perp_parameters_args,
     update_pricing_parameters_args,
     update_state_args,
-    update_volatility_args,
-    update_zeta_group_expiry_args,
     update_zeta_pricing_pubkeys_args,
     validation_type,
 )
 from .anchor_decimal import AnchorDecimal, AnchorDecimalJSON
 from .asset import AssetJSON, AssetKind
 from .cross_margin_account_info import (
     CrossMarginAccountInfo,
     CrossMarginAccountInfoJSON,
 )
-from .expire_series_override_args import (
-    ExpireSeriesOverrideArgs,
-    ExpireSeriesOverrideArgsJSON,
-)
-from .expiry_series import ExpirySeries, ExpirySeriesJSON
-from .expiry_series_status import ExpirySeriesStatusJSON, ExpirySeriesStatusKind
 from .halt_args import HaltArgs, HaltArgsJSON
 from .halt_state import HaltState, HaltStateJSON
 from .halt_state_args import HaltStateArgs, HaltStateArgsJSON
 from .halt_state_v2 import HaltStateV2, HaltStateV2JSON
 from .initialize_market_args import InitializeMarketArgs, InitializeMarketArgsJSON
 from .initialize_market_node_args import (
     InitializeMarketNodeArgs,
     InitializeMarketNodeArgsJSON,
 )
 from .initialize_state_args import InitializeStateArgs, InitializeStateArgsJSON
-from .initialize_zeta_group_args import (
-    InitializeZetaGroupArgs,
-    InitializeZetaGroupArgsJSON,
-)
 from .initialize_zeta_pricing_args import (
     InitializeZetaPricingArgs,
     InitializeZetaPricingArgsJSON,
 )
 from .kind import KindJSON, KindKind
 from .margin_account_type import MarginAccountTypeJSON, MarginAccountTypeKind
 from .margin_parameters import MarginParameters, MarginParametersJSON
 from .margin_requirement import MarginRequirementJSON, MarginRequirementKind
 from .movement_type import MovementTypeJSON, MovementTypeKind
 from .order_complete_type import OrderCompleteTypeJSON, OrderCompleteTypeKind
 from .order_state import OrderState, OrderStateJSON
 from .order_type import OrderTypeJSON, OrderTypeKind
-from .override_expiry_args import OverrideExpiryArgs, OverrideExpiryArgsJSON
 from .perp_parameters import PerpParameters, PerpParametersJSON
 from .place_order_type import PlaceOrderTypeJSON, PlaceOrderTypeKind
 from .position import Position, PositionJSON
-from .position_movement_arg import PositionMovementArg, PositionMovementArgJSON
 from .pricing_parameters import PricingParameters, PricingParametersJSON
 from .product import Product, ProductJSON
 from .product_greeks import ProductGreeks, ProductGreeksJSON
 from .product_ledger import ProductLedger, ProductLedgerJSON
 from .set_referrals_rewards_args import (
     SetReferralsRewardsArgs,
     SetReferralsRewardsArgsJSON,
 )
 from .side import SideJSON, SideKind
 from .strike import Strike, StrikeJSON
 from .trait_type import TraitTypeJSON, TraitTypeKind
 from .treasury_movement_type import TreasuryMovementTypeJSON, TreasuryMovementTypeKind
-from .update_greeks_args import UpdateGreeksArgs, UpdateGreeksArgsJSON
-from .update_interest_rate_args import (
-    UpdateInterestRateArgs,
-    UpdateInterestRateArgsJSON,
-)
 from .update_margin_parameters_args import (
     UpdateMarginParametersArgs,
     UpdateMarginParametersArgsJSON,
 )
 from .update_perp_parameters_args import (
     UpdatePerpParametersArgs,
     UpdatePerpParametersArgsJSON,
 )
 from .update_pricing_parameters_args import (
     UpdatePricingParametersArgs,
     UpdatePricingParametersArgsJSON,
 )
 from .update_state_args import UpdateStateArgs, UpdateStateArgsJSON
-from .update_volatility_args import UpdateVolatilityArgs, UpdateVolatilityArgsJSON
-from .update_zeta_group_expiry_args import (
-    UpdateZetaGroupExpiryArgs,
-    UpdateZetaGroupExpiryArgsJSON,
-)
 from .update_zeta_pricing_pubkeys_args import (
     UpdateZetaPricingPubkeysArgs,
     UpdateZetaPricingPubkeysArgsJSON,
 )
 from .validation_type import ValidationTypeJSON, ValidationTypeKind
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/__init__.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/anchor_decimal.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/anchor_decimal.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/anchor_decimal.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/anchor_decimal.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/asset.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/asset.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/asset.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/kind.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Oct 24 12:06:35 2023 UTC, .py size: 4212 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,367 +1,283 @@
-00000000: 610d 0d0a 0000 0000 4bb3 3765 7410 0000  a.......K.7et...
+00000000: 610d 0d0a 0000 0000 1f64 e364 f80c 0000  a........d.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000a 0000 0040 0000 0173 d001 0000 6400  .....@...s....d.
+00000020: 0008 0000 0040 0000 0173 6c01 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6402 6c05 5a06 6400 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6502 6a09  ..G.d.d...d.e.j.
 00000070: 8303 5a0a 4700 6407 6408 8400 6408 6502  ..Z.G.d.d...d.e.
 00000080: 6a09 8303 5a0b 4700 6409 640a 8400 640a  j...Z.G.d.d...d.
 00000090: 6502 6a09 8303 5a0c 4700 640b 640c 8400  e.j...Z.G.d.d...
 000000a0: 640c 6502 6a09 8303 5a0d 4700 640d 640e  d.e.j...Z.G.d.d.
-000000b0: 8400 640e 6502 6a09 8303 5a0e 4700 640f  ..d.e.j...Z.G.d.
-000000c0: 6410 8400 6410 6502 6a09 8303 5a0f 4700  d...d.e.j...Z.G.
-000000d0: 6411 6412 8400 6412 6502 6a09 8303 5a10  d.d...d.e.j...Z.
+000000b0: 8400 640e 6502 6a09 8303 5a0e 6504 4700  ..d.e.j...Z.e.G.
+000000c0: 640f 6410 8400 6410 8302 8301 5a0f 6504  d.d...d.....Z.e.
+000000d0: 4700 6411 6412 8400 6412 8302 8301 5a10  G.d.d...d.....Z.
 000000e0: 6504 4700 6413 6414 8400 6414 8302 8301  e.G.d.d...d.....
 000000f0: 5a11 6504 4700 6415 6416 8400 6416 8302  Z.e.G.d.d...d...
 00000100: 8301 5a12 6504 4700 6417 6418 8400 6418  ..Z.e.G.d.d...d.
-00000110: 8302 8301 5a13 6504 4700 6419 641a 8400  ....Z.e.G.d.d...
-00000120: 641a 8302 8301 5a14 6504 4700 641b 641c  d.....Z.e.G.d.d.
-00000130: 8400 641c 8302 8301 5a15 6504 4700 641d  ..d.....Z.e.G.d.
-00000140: 641e 8400 641e 8302 8301 5a16 6504 4700  d...d.....Z.e.G.
-00000150: 641f 6420 8400 6420 8302 8301 5a17 6502  d.d ..d ....Z.e.
-00000160: 6a18 6511 6512 6513 6514 6515 6516 6517  j.e.e.e.e.e.e.e.
-00000170: 6607 1900 5a19 6502 6a18 650a 650b 650c  f...Z.e.j.e.e.e.
-00000180: 650d 650e 650f 6510 6607 1900 5a1a 6421  e.e.e.e.f...Z.d!
-00000190: 6422 6423 9c02 6424 6425 8404 5a1b 6426  d"d#..d$d%..Z.d&
-000001a0: 6422 6423 9c02 6427 6428 8404 5a1c 6508  d"d#..d'd(..Z.e.
-000001b0: 6414 6506 a01d a100 1b00 6416 6506 a01d  d.e.......d.e...
-000001c0: a100 1b00 6418 6506 a01d a100 1b00 641a  ....d.e.......d.
-000001d0: 6506 a01d a100 1b00 641c 6506 a01d a100  e.......d.e.....
-000001e0: 1b00 641e 6506 a01d a100 1b00 6420 6506  ..d.e.......d e.
-000001f0: a01d a100 1b00 8307 5a1e 6402 5300 2929  ........Z.d.S.))
-00000200: e900 0000 0029 01da 0b61 6e6e 6f74 6174  .....)...annotat
-00000210: 696f 6e73 4e29 01da 0964 6174 6163 6c61  ionsN)...datacla
-00000220: 7373 2901 da0e 456e 756d 466f 7243 6f64  ss)...EnumForCod
-00000230: 6567 656e 6300 0000 0000 0000 0000 0000  egenc...........
-00000240: 0000 0000 0003 0000 0040 0000 0173 1600  .........@...s..
-00000250: 0000 6500 5a01 6400 5a02 5500 6401 6503  ..e.Z.d.Z.U.d.e.
-00000260: 6402 3c00 6403 5300 2904 da07 534f 4c4a  d.<.d.S.)...SOLJ
-00000270: 534f 4e7a 1574 7970 696e 672e 4c69 7465  SONz.typing.Lite
-00000280: 7261 6c5b 2753 4f4c 275d da04 6b69 6e64  ral['SOL']..kind
-00000290: 4ea9 04da 085f 5f6e 616d 655f 5fda 0a5f  N....__name__.._
-000002a0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-000002b0: 6c6e 616d 655f 5fda 0f5f 5f61 6e6e 6f74  lname__..__annot
-000002c0: 6174 696f 6e73 5f5f a900 720c 0000 0072  ations__..r....r
-000002d0: 0c00 0000 fa56 2f55 7365 7273 2f74 6672  .....V/Users/tfr
-000002e0: 697a 7a61 2f44 6f63 756d 656e 7473 2f7a  izza/Documents/z
-000002f0: 6574 612f 7a65 7461 6d61 726b 6574 732d  eta/zetamarkets-
-00000300: 7079 2f7a 6574 616d 6172 6b65 7473 5f70  py/zetamarkets_p
-00000310: 792f 7a65 7461 5f63 6c69 656e 742f 7479  y/zeta_client/ty
-00000320: 7065 732f 6173 7365 742e 7079 7205 0000  pes/asset.pyr...
-00000330: 000a 0000 0073 0200 0000 0a01 7205 0000  .....s......r...
-00000340: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000350: 0000 0300 0000 4000 0001 7316 0000 0065  ......@...s....e
-00000360: 005a 0164 005a 0255 0064 0165 0364 023c  .Z.d.Z.U.d.e.d.<
-00000370: 0064 0353 0029 04da 0742 5443 4a53 4f4e  .d.S.)...BTCJSON
-00000380: 7a15 7479 7069 6e67 2e4c 6974 6572 616c  z.typing.Literal
-00000390: 5b27 4254 4327 5d72 0600 0000 4e72 0700  ['BTC']r....Nr..
-000003a0: 0000 720c 0000 0072 0c00 0000 720c 0000  ..r....r....r...
-000003b0: 0072 0d00 0000 720e 0000 000e 0000 0073  .r....r........s
-000003c0: 0200 0000 0a01 720e 0000 0063 0000 0000  ......r....c....
-000003d0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-000003e0: 4000 0001 7316 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-000003f0: 0255 0064 0165 0364 023c 0064 0353 0029  .U.d.e.d.<.d.S.)
-00000400: 04da 0745 5448 4a53 4f4e 7a15 7479 7069  ...ETHJSONz.typi
-00000410: 6e67 2e4c 6974 6572 616c 5b27 4554 4827  ng.Literal['ETH'
-00000420: 5d72 0600 0000 4e72 0700 0000 720c 0000  ]r....Nr....r...
-00000430: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00000440: 720f 0000 0012 0000 0073 0200 0000 0a01  r........s......
-00000450: 720f 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000460: 0000 0000 0000 0300 0000 4000 0001 7316  ..........@...s.
-00000470: 0000 0065 005a 0164 005a 0255 0064 0165  ...e.Z.d.Z.U.d.e
-00000480: 0364 023c 0064 0353 0029 04da 0741 5054  .d.<.d.S.)...APT
-00000490: 4a53 4f4e 7a15 7479 7069 6e67 2e4c 6974  JSONz.typing.Lit
-000004a0: 6572 616c 5b27 4150 5427 5d72 0600 0000  eral['APT']r....
-000004b0: 4e72 0700 0000 720c 0000 0072 0c00 0000  Nr....r....r....
-000004c0: 720c 0000 0072 0d00 0000 7210 0000 0016  r....r....r.....
-000004d0: 0000 0073 0200 0000 0a01 7210 0000 0063  ...s......r....c
-000004e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004f0: 0300 0000 4000 0001 7316 0000 0065 005a  ....@...s....e.Z
-00000500: 0164 005a 0255 0064 0165 0364 023c 0064  .d.Z.U.d.e.d.<.d
-00000510: 0353 0029 04da 0741 5242 4a53 4f4e 7a15  .S.)...ARBJSONz.
-00000520: 7479 7069 6e67 2e4c 6974 6572 616c 5b27  typing.Literal['
-00000530: 4152 4227 5d72 0600 0000 4e72 0700 0000  ARB']r....Nr....
-00000540: 720c 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
-00000550: 0d00 0000 7211 0000 001a 0000 0073 0200  ....r........s..
-00000560: 0000 0a01 7211 0000 0063 0000 0000 0000  ....r....c......
-00000570: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00000580: 0001 7316 0000 0065 005a 0164 005a 0255  ..s....e.Z.d.Z.U
-00000590: 0064 0165 0364 023c 0064 0353 0029 04da  .d.e.d.<.d.S.)..
-000005a0: 0742 4e42 4a53 4f4e 7a15 7479 7069 6e67  .BNBJSONz.typing
-000005b0: 2e4c 6974 6572 616c 5b27 424e 4227 5d72  .Literal['BNB']r
-000005c0: 0600 0000 4e72 0700 0000 720c 0000 0072  ....Nr....r....r
-000005d0: 0c00 0000 720c 0000 0072 0d00 0000 7212  ....r....r....r.
-000005e0: 0000 001e 0000 0073 0200 0000 0a01 7212  .......s......r.
-000005f0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000600: 0000 0000 0300 0000 4000 0001 7316 0000  ........@...s...
-00000610: 0065 005a 0164 005a 0255 0064 0165 0364  .e.Z.d.Z.U.d.e.d
-00000620: 023c 0064 0353 0029 04da 0d55 4e44 4546  .<.d.S.)...UNDEF
-00000630: 494e 4544 4a53 4f4e 7a1b 7479 7069 6e67  INEDJSONz.typing
-00000640: 2e4c 6974 6572 616c 5b27 554e 4445 4649  .Literal['UNDEFI
-00000650: 4e45 4427 5d72 0600 0000 4e72 0700 0000  NED']r....Nr....
-00000660: 720c 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
-00000670: 0d00 0000 7213 0000 0022 0000 0073 0200  ....r...."...s..
-00000680: 0000 0a01 7213 0000 0063 0000 0000 0000  ....r....c......
-00000690: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
-000006a0: 0001 734a 0000 0065 005a 0164 005a 0255  ..sJ...e.Z.d.Z.U
-000006b0: 0064 015a 0364 0265 0464 033c 0064 005a  .d.Z.d.e.d.<.d.Z
-000006c0: 0564 0265 0464 043c 0065 0664 0564 069c  .d.e.d.<.e.d.d..
-000006d0: 0164 0764 0884 0483 015a 0765 0664 0964  .d.d.....Z.e.d.d
-000006e0: 069c 0164 0a64 0b84 0483 015a 0864 0c53  ...d.d.....Z.d.S
-000006f0: 0029 0dda 0353 4f4c 7201 0000 00fa 0f74  .)...SOLr......t
-00000700: 7970 696e 672e 436c 6173 7356 6172 da0d  yping.ClassVar..
-00000710: 6469 7363 7269 6d69 6e61 746f 7272 0600  discriminatorr..
-00000720: 0000 7205 0000 00a9 01da 0672 6574 7572  ..r........retur
-00000730: 6e63 0100 0000 0000 0000 0000 0000 0100  nc..............
-00000740: 0000 0300 0000 4300 0001 730a 0000 0074  ......C...s....t
-00000750: 0064 0164 028d 0153 0029 034e 7214 0000  .d.d...S.).Nr...
-00000760: 00a9 0172 0600 0000 2901 7205 0000 00a9  ...r....).r.....
-00000770: 01da 0363 6c73 720c 0000 0072 0c00 0000  ...clsr....r....
-00000780: 720d 0000 00da 0774 6f5f 6a73 6f6e 2b00  r......to_json+.
-00000790: 0000 7306 0000 0000 0202 0102 ff7a 0b53  ..s..........z.S
-000007a0: 4f4c 2e74 6f5f 6a73 6f6e da04 6469 6374  OL.to_json..dict
-000007b0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000007c0: 0002 0000 0043 0000 0173 0800 0000 6401  .....C...s....d.
-000007d0: 6900 6901 5300 2902 4e72 1400 0000 720c  i.i.S.).Nr....r.
-000007e0: 0000 0072 1a00 0000 720c 0000 0072 0c00  ...r....r....r..
-000007f0: 0000 720d 0000 00da 0c74 6f5f 656e 636f  ..r......to_enco
-00000800: 6461 626c 6531 0000 0073 0400 0000 0003  dable1...s......
-00000810: 04ff 7a10 534f 4c2e 746f 5f65 6e63 6f64  ..z.SOL.to_encod
-00000820: 6162 6c65 4ea9 0972 0800 0000 7209 0000  ableN..r....r...
-00000830: 0072 0a00 0000 7216 0000 0072 0b00 0000  .r....r....r....
-00000840: 7206 0000 00da 0b63 6c61 7373 6d65 7468  r......classmeth
-00000850: 6f64 721c 0000 0072 1e00 0000 720c 0000  odr....r....r...
-00000860: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00000870: 7214 0000 0026 0000 0073 0c00 0000 0a02  r....&...s......
-00000880: 0c01 0c02 0201 1005 0201 7214 0000 0063  ..........r....c
-00000890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000008a0: 0400 0000 4000 0001 734a 0000 0065 005a  ....@...sJ...e.Z
-000008b0: 0164 005a 0255 0064 015a 0364 0265 0464  .d.Z.U.d.Z.d.e.d
-000008c0: 033c 0064 005a 0564 0265 0464 043c 0065  .<.d.Z.d.e.d.<.e
-000008d0: 0664 0564 069c 0164 0764 0884 0483 015a  .d.d...d.d.....Z
-000008e0: 0765 0664 0964 069c 0164 0a64 0b84 0483  .e.d.d...d.d....
-000008f0: 015a 0864 0c53 0029 0dda 0342 5443 e901  .Z.d.S.)...BTC..
-00000900: 0000 0072 1500 0000 7216 0000 0072 0600  ...r....r....r..
-00000910: 0000 720e 0000 0072 1700 0000 6301 0000  ..r....r....c...
-00000920: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00000930: 0043 0000 0173 0a00 0000 7400 6401 6402  .C...s....t.d.d.
-00000940: 8d01 5300 2903 4e72 2100 0000 7219 0000  ..S.).Nr!...r...
-00000950: 0029 0172 0e00 0000 721a 0000 0072 0c00  .).r....r....r..
-00000960: 0000 720c 0000 0072 0d00 0000 721c 0000  ..r....r....r...
-00000970: 003d 0000 0073 0600 0000 0002 0201 02ff  .=...s..........
-00000980: 7a0b 4254 432e 746f 5f6a 736f 6e72 1d00  z.BTC.to_jsonr..
-00000990: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-000009a0: 0000 0002 0000 0043 0000 0173 0800 0000  .......C...s....
-000009b0: 6401 6900 6901 5300 2902 4e72 2100 0000  d.i.i.S.).Nr!...
-000009c0: 720c 0000 0072 1a00 0000 720c 0000 0072  r....r....r....r
-000009d0: 0c00 0000 720d 0000 0072 1e00 0000 4300  ....r....r....C.
-000009e0: 0000 7304 0000 0000 0304 ff7a 1042 5443  ..s........z.BTC
-000009f0: 2e74 6f5f 656e 636f 6461 626c 654e 721f  .to_encodableNr.
-00000a00: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
-00000a10: 0000 720d 0000 0072 2100 0000 3800 0000  ..r....r!...8...
-00000a20: 730c 0000 000a 020c 010c 0202 0110 0502  s...............
-00000a30: 0172 2100 0000 6300 0000 0000 0000 0000  .r!...c.........
-00000a40: 0000 0000 0000 0004 0000 0040 0000 0173  ...........@...s
-00000a50: 4a00 0000 6500 5a01 6400 5a02 5500 6401  J...e.Z.d.Z.U.d.
-00000a60: 5a03 6402 6504 6403 3c00 6400 5a05 6402  Z.d.e.d.<.d.Z.d.
-00000a70: 6504 6404 3c00 6506 6405 6406 9c01 6407  e.d.<.e.d.d...d.
-00000a80: 6408 8404 8301 5a07 6506 6409 6406 9c01  d.....Z.e.d.d...
-00000a90: 640a 640b 8404 8301 5a08 640c 5300 290d  d.d.....Z.d.S.).
-00000aa0: da03 4554 48e9 0200 0000 7215 0000 0072  ..ETH.....r....r
-00000ab0: 1600 0000 7206 0000 0072 0f00 0000 7217  ....r....r....r.
-00000ac0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000ad0: 0100 0000 0300 0000 4300 0001 730a 0000  ........C...s...
-00000ae0: 0074 0064 0164 028d 0153 0029 034e 7223  .t.d.d...S.).Nr#
-00000af0: 0000 0072 1900 0000 2901 720f 0000 0072  ...r....).r....r
-00000b00: 1a00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-00000b10: 0000 0072 1c00 0000 4f00 0000 7306 0000  ...r....O...s...
-00000b20: 0000 0202 0102 ff7a 0b45 5448 2e74 6f5f  .......z.ETH.to_
-00000b30: 6a73 6f6e 721d 0000 0063 0100 0000 0000  jsonr....c......
-00000b40: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00000b50: 0001 7308 0000 0064 0169 0069 0153 0029  ..s....d.i.i.S.)
-00000b60: 024e 7223 0000 0072 0c00 0000 721a 0000  .Nr#...r....r...
-00000b70: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00000b80: 721e 0000 0055 0000 0073 0400 0000 0003  r....U...s......
-00000b90: 04ff 7a10 4554 482e 746f 5f65 6e63 6f64  ..z.ETH.to_encod
-00000ba0: 6162 6c65 4e72 1f00 0000 720c 0000 0072  ableNr....r....r
-00000bb0: 0c00 0000 720c 0000 0072 0d00 0000 7223  ....r....r....r#
-00000bc0: 0000 004a 0000 0073 0c00 0000 0a02 0c01  ...J...s........
-00000bd0: 0c02 0201 1005 0201 7223 0000 0063 0000  ........r#...c..
-00000be0: 0000 0000 0000 0000 0000 0000 0000 0400  ................
-00000bf0: 0000 4000 0001 734a 0000 0065 005a 0164  ..@...sJ...e.Z.d
-00000c00: 005a 0255 0064 015a 0364 0265 0464 033c  .Z.U.d.Z.d.e.d.<
-00000c10: 0064 005a 0564 0265 0464 043c 0065 0664  .d.Z.d.e.d.<.e.d
-00000c20: 0564 069c 0164 0764 0884 0483 015a 0765  .d...d.d.....Z.e
-00000c30: 0664 0964 069c 0164 0a64 0b84 0483 015a  .d.d...d.d.....Z
-00000c40: 0864 0c53 0029 0dda 0341 5054 e903 0000  .d.S.)...APT....
-00000c50: 0072 1500 0000 7216 0000 0072 0600 0000  .r....r....r....
-00000c60: 7210 0000 0072 1700 0000 6301 0000 0000  r....r....c.....
-00000c70: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00000c80: 0000 0173 0a00 0000 7400 6401 6402 8d01  ...s....t.d.d...
-00000c90: 5300 2903 4e72 2500 0000 7219 0000 0029  S.).Nr%...r....)
-00000ca0: 0172 1000 0000 721a 0000 0072 0c00 0000  .r....r....r....
-00000cb0: 720c 0000 0072 0d00 0000 721c 0000 0061  r....r....r....a
-00000cc0: 0000 0073 0600 0000 0002 0201 02ff 7a0b  ...s..........z.
-00000cd0: 4150 542e 746f 5f6a 736f 6e72 1d00 0000  APT.to_jsonr....
-00000ce0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000cf0: 0002 0000 0043 0000 0173 0800 0000 6401  .....C...s....d.
-00000d00: 6900 6901 5300 2902 4e72 2500 0000 720c  i.i.S.).Nr%...r.
-00000d10: 0000 0072 1a00 0000 720c 0000 0072 0c00  ...r....r....r..
-00000d20: 0000 720d 0000 0072 1e00 0000 6700 0000  ..r....r....g...
-00000d30: 7304 0000 0000 0304 ff7a 1041 5054 2e74  s........z.APT.t
-00000d40: 6f5f 656e 636f 6461 626c 654e 721f 0000  o_encodableNr...
-00000d50: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
-00000d60: 720d 0000 0072 2500 0000 5c00 0000 730c  r....r%...\...s.
-00000d70: 0000 000a 020c 010c 0202 0110 0502 0172  ...............r
-00000d80: 2500 0000 6300 0000 0000 0000 0000 0000  %...c...........
-00000d90: 0000 0000 0004 0000 0040 0000 0173 4a00  .........@...sJ.
-00000da0: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
-00000db0: 6402 6504 6403 3c00 6400 5a05 6402 6504  d.e.d.<.d.Z.d.e.
-00000dc0: 6404 3c00 6506 6405 6406 9c01 6407 6408  d.<.e.d.d...d.d.
-00000dd0: 8404 8301 5a07 6506 6409 6406 9c01 640a  ....Z.e.d.d...d.
-00000de0: 640b 8404 8301 5a08 640c 5300 290d da03  d.....Z.d.S.)...
-00000df0: 4152 42e9 0400 0000 7215 0000 0072 1600  ARB.....r....r..
-00000e00: 0000 7206 0000 0072 1100 0000 7217 0000  ..r....r....r...
-00000e10: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00000e20: 0000 0300 0000 4300 0001 730a 0000 0074  ......C...s....t
-00000e30: 0064 0164 028d 0153 0029 034e 7227 0000  .d.d...S.).Nr'..
-00000e40: 0072 1900 0000 2901 7211 0000 0072 1a00  .r....).r....r..
-00000e50: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00000e60: 0072 1c00 0000 7300 0000 7306 0000 0000  .r....s...s.....
-00000e70: 0202 0102 ff7a 0b41 5242 2e74 6f5f 6a73  .....z.ARB.to_js
-00000e80: 6f6e 721d 0000 0063 0100 0000 0000 0000  onr....c........
-00000e90: 0000 0000 0100 0000 0200 0000 4300 0001  ............C...
-00000ea0: 7308 0000 0064 0169 0069 0153 0029 024e  s....d.i.i.S.).N
-00000eb0: 7227 0000 0072 0c00 0000 721a 0000 0072  r'...r....r....r
-00000ec0: 0c00 0000 720c 0000 0072 0d00 0000 721e  ....r....r....r.
-00000ed0: 0000 0079 0000 0073 0400 0000 0003 04ff  ...y...s........
-00000ee0: 7a10 4152 422e 746f 5f65 6e63 6f64 6162  z.ARB.to_encodab
-00000ef0: 6c65 4e72 1f00 0000 720c 0000 0072 0c00  leNr....r....r..
-00000f00: 0000 720c 0000 0072 0d00 0000 7227 0000  ..r....r....r'..
-00000f10: 006e 0000 0073 0c00 0000 0a02 0c01 0c02  .n...s..........
-00000f20: 0201 1005 0201 7227 0000 0063 0000 0000  ......r'...c....
-00000f30: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00000f40: 4000 0001 734a 0000 0065 005a 0164 005a  @...sJ...e.Z.d.Z
-00000f50: 0255 0064 015a 0364 0265 0464 033c 0064  .U.d.Z.d.e.d.<.d
-00000f60: 005a 0564 0265 0464 043c 0065 0664 0564  .Z.d.e.d.<.e.d.d
-00000f70: 069c 0164 0764 0884 0483 015a 0765 0664  ...d.d.....Z.e.d
-00000f80: 0964 069c 0164 0a64 0b84 0483 015a 0864  .d...d.d.....Z.d
-00000f90: 0c53 0029 0dda 0342 4e42 e905 0000 0072  .S.)...BNB.....r
-00000fa0: 1500 0000 7216 0000 0072 0600 0000 7212  ....r....r....r.
-00000fb0: 0000 0072 1700 0000 6301 0000 0000 0000  ...r....c.......
-00000fc0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00000fd0: 0173 0a00 0000 7400 6401 6402 8d01 5300  .s....t.d.d...S.
-00000fe0: 2903 4e72 2900 0000 7219 0000 0029 0172  ).Nr)...r....).r
-00000ff0: 1200 0000 721a 0000 0072 0c00 0000 720c  ....r....r....r.
-00001000: 0000 0072 0d00 0000 721c 0000 0085 0000  ...r....r.......
-00001010: 0073 0600 0000 0002 0201 02ff 7a0b 424e  .s..........z.BN
-00001020: 422e 746f 5f6a 736f 6e72 1d00 0000 6301  B.to_jsonr....c.
-00001030: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00001040: 0000 0043 0000 0173 0800 0000 6401 6900  ...C...s....d.i.
-00001050: 6901 5300 2902 4e72 2900 0000 720c 0000  i.S.).Nr)...r...
-00001060: 0072 1a00 0000 720c 0000 0072 0c00 0000  .r....r....r....
-00001070: 720d 0000 0072 1e00 0000 8b00 0000 7304  r....r........s.
-00001080: 0000 0000 0304 ff7a 1042 4e42 2e74 6f5f  .......z.BNB.to_
-00001090: 656e 636f 6461 626c 654e 721f 0000 0072  encodableNr....r
-000010a0: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-000010b0: 0000 0072 2900 0000 8000 0000 730c 0000  ...r).......s...
-000010c0: 000a 020c 010c 0202 0110 0502 0172 2900  .............r).
-000010d0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000010e0: 0000 0004 0000 0040 0000 0173 4a00 0000  .......@...sJ...
-000010f0: 6500 5a01 6400 5a02 5500 6401 5a03 6402  e.Z.d.Z.U.d.Z.d.
-00001100: 6504 6403 3c00 6400 5a05 6402 6504 6404  e.d.<.d.Z.d.e.d.
-00001110: 3c00 6506 6405 6406 9c01 6407 6408 8404  <.e.d.d...d.d...
-00001120: 8301 5a07 6506 6409 6406 9c01 640a 640b  ..Z.e.d.d...d.d.
-00001130: 8404 8301 5a08 640c 5300 290d da09 554e  ....Z.d.S.)...UN
-00001140: 4445 4649 4e45 4472 2a00 0000 7215 0000  DEFINEDr*...r...
-00001150: 0072 1600 0000 7206 0000 0072 1300 0000  .r....r....r....
-00001160: 7217 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00001170: 0000 0100 0000 0300 0000 4300 0001 730a  ..........C...s.
-00001180: 0000 0074 0064 0164 028d 0153 0029 034e  ...t.d.d...S.).N
-00001190: 722b 0000 0072 1900 0000 2901 7213 0000  r+...r....).r...
-000011a0: 0072 1a00 0000 720c 0000 0072 0c00 0000  .r....r....r....
-000011b0: 720d 0000 0072 1c00 0000 9700 0000 7306  r....r........s.
-000011c0: 0000 0000 0202 0102 ff7a 1155 4e44 4546  .........z.UNDEF
-000011d0: 494e 4544 2e74 6f5f 6a73 6f6e 721d 0000  INED.to_jsonr...
-000011e0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-000011f0: 0000 0200 0000 4300 0001 7308 0000 0064  ......C...s....d
-00001200: 0169 0069 0153 0029 024e 722b 0000 0072  .i.i.S.).Nr+...r
-00001210: 0c00 0000 721a 0000 0072 0c00 0000 720c  ....r....r....r.
-00001220: 0000 0072 0d00 0000 721e 0000 009d 0000  ...r....r.......
-00001230: 0073 0400 0000 0003 04ff 7a16 554e 4445  .s........z.UNDE
-00001240: 4649 4e45 442e 746f 5f65 6e63 6f64 6162  FINED.to_encodab
-00001250: 6c65 4e72 1f00 0000 720c 0000 0072 0c00  leNr....r....r..
-00001260: 0000 720c 0000 0072 0d00 0000 722b 0000  ..r....r....r+..
-00001270: 0092 0000 0073 0c00 0000 0a02 0c01 0c02  .....s..........
-00001280: 0201 1005 0201 722b 0000 0072 1d00 0000  ......r+...r....
-00001290: da09 4173 7365 744b 696e 6429 02da 036f  ..AssetKind)...o
-000012a0: 626a 7218 0000 0063 0100 0000 0000 0000  bjr....c........
-000012b0: 0000 0000 0100 0000 0300 0000 4300 0001  ............C...
-000012c0: 7380 0000 0074 007c 0074 0183 0273 1274  s....t.|.t...s.t
-000012d0: 0264 0183 0182 0164 027c 0076 0072 2074  .d.....d.|.v.r t
-000012e0: 0383 0053 0064 037c 0076 0072 2e74 0483  ...S.d.|.v.r.t..
-000012f0: 0053 0064 047c 0076 0072 3c74 0583 0053  .S.d.|.v.r<t...S
-00001300: 0064 057c 0076 0072 4a74 0683 0053 0064  .d.|.v.rJt...S.d
-00001310: 067c 0076 0072 5874 0783 0053 0064 077c  .|.v.rXt...S.d.|
-00001320: 0076 0072 6674 0883 0053 0064 087c 0076  .v.rft...S.d.|.v
-00001330: 0072 7474 0983 0053 0074 0264 0183 0182  .rtt...S.t.d....
-00001340: 0164 0053 0029 094e 7a13 496e 7661 6c69  .d.S.).Nz.Invali
-00001350: 6420 656e 756d 206f 626a 6563 7472 1400  d enum objectr..
-00001360: 0000 7221 0000 0072 2300 0000 7225 0000  ..r!...r#...r%..
-00001370: 0072 2700 0000 7229 0000 0072 2b00 0000  .r'...r)...r+...
-00001380: 290a da0a 6973 696e 7374 616e 6365 721d  )...isinstancer.
-00001390: 0000 00da 0a56 616c 7565 4572 726f 7272  .....ValueErrorr
-000013a0: 1400 0000 7221 0000 0072 2300 0000 7225  ....r!...r#...r%
-000013b0: 0000 0072 2700 0000 7229 0000 0072 2b00  ...r'...r)...r+.
-000013c0: 0000 2901 722d 0000 0072 0c00 0000 720c  ..).r-...r....r.
-000013d0: 0000 0072 0d00 0000 da0c 6672 6f6d 5f64  ...r......from_d
-000013e0: 6563 6f64 6564 a800 0000 7322 0000 0000  ecoded....s"....
-000013f0: 010a 0108 0108 0106 0108 0106 0108 0106  ................
-00001400: 0108 0106 0108 0106 0108 0106 0108 0106  ................
-00001410: 0172 3000 0000 da09 4173 7365 744a 534f  .r0.....AssetJSO
-00001420: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
-00001430: 0000 0300 0000 4300 0001 7398 0000 007c  ......C...s....|
-00001440: 0064 0119 0064 026b 0272 1274 0083 0053  .d...d.k.r.t...S
-00001450: 007c 0064 0119 0064 036b 0272 2474 0183  .|.d...d.k.r$t..
-00001460: 0053 007c 0064 0119 0064 046b 0272 3674  .S.|.d...d.k.r6t
-00001470: 0283 0053 007c 0064 0119 0064 056b 0272  ...S.|.d...d.k.r
-00001480: 4874 0383 0053 007c 0064 0119 0064 066b  Ht...S.|.d...d.k
-00001490: 0272 5a74 0483 0053 007c 0064 0119 0064  .rZt...S.|.d...d
-000014a0: 076b 0272 6c74 0583 0053 007c 0064 0119  .k.rlt...S.|.d..
-000014b0: 0064 086b 0272 7e74 0683 0053 007c 0064  .d.k.r~t...S.|.d
-000014c0: 0119 007d 0174 0764 097c 019b 009d 0283  ...}.t.d.|......
-000014d0: 0182 0164 0053 0029 0a4e 7206 0000 0072  ...d.S.).Nr....r
-000014e0: 1400 0000 7221 0000 0072 2300 0000 7225  ....r!...r#...r%
-000014f0: 0000 0072 2700 0000 7229 0000 0072 2b00  ...r'...r)...r+.
-00001500: 0000 7a18 556e 7265 636f 676e 697a 6564  ..z.Unrecognized
-00001510: 2065 6e75 6d20 6b69 6e64 3a20 2908 7214   enum kind: ).r.
-00001520: 0000 0072 2100 0000 7223 0000 0072 2500  ...r!...r#...r%.
-00001530: 0000 7227 0000 0072 2900 0000 722b 0000  ..r'...r)...r+..
-00001540: 0072 2f00 0000 2902 722d 0000 0072 0600  .r/...).r-...r..
-00001550: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00001560: 00da 0966 726f 6d5f 6a73 6f6e bc00 0000  ...from_json....
-00001570: 7320 0000 0000 010c 0106 010c 0106 010c  s ..............
-00001580: 0106 010c 0106 010c 0106 010c 0106 010c  ................
-00001590: 0106 0108 0172 3200 0000 291f da0a 5f5f  .....r2...)...__
-000015a0: 6675 7475 7265 5f5f 7202 0000 00da 0674  future__r......t
-000015b0: 7970 696e 67da 0b64 6174 6163 6c61 7373  yping..dataclass
-000015c0: 6573 7203 0000 00da 0f62 6f72 7368 5f63  esr......borsh_c
-000015d0: 6f6e 7374 7275 6374 da05 626f 7273 68da  onstruct..borsh.
-000015e0: 1861 6e63 686f 7270 792e 626f 7273 685f  .anchorpy.borsh_
-000015f0: 6578 7465 6e73 696f 6e72 0400 0000 da09  extensionr......
-00001600: 5479 7065 6444 6963 7472 0500 0000 720e  TypedDictr....r.
-00001610: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
-00001620: 0000 7212 0000 0072 1300 0000 7214 0000  ..r....r....r...
-00001630: 0072 2100 0000 7223 0000 0072 2500 0000  .r!...r#...r%...
-00001640: 7227 0000 0072 2900 0000 722b 0000 00da  r'...r)...r+....
-00001650: 0555 6e69 6f6e 722c 0000 0072 3100 0000  .Unionr,...r1...
-00001660: 7230 0000 0072 3200 0000 da07 4353 7472  r0...r2.....CStr
-00001670: 7563 74da 066c 6179 6f75 7472 0c00 0000  uct..layoutr....
-00001680: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00001690: 083c 6d6f 6475 6c65 3e01 0000 0073 4c00  .<module>....sL.
-000016a0: 0000 0c02 0801 0c02 0801 0c03 1204 1204  ................
-000016b0: 1204 1204 1204 1204 1204 0201 1011 0201  ................
-000016c0: 1011 0201 1011 0201 1011 0201 1011 0201  ................
-000016d0: 1011 0201 1011 1801 1803 1014 1013 0201  ................
-000016e0: 0a01 0a01 0a01 0a01 0a01 0a01 0af9       ..............
+00000110: 8302 8301 5a13 6502 6a14 650f 6510 6511  ....Z.e.j.e.e.e.
+00000120: 6512 6513 6605 1900 5a15 6502 6a14 650a  e.e.f...Z.e.j.e.
+00000130: 650b 650c 650d 650e 6605 1900 5a16 6419  e.e.e.e.f...Z.d.
+00000140: 641a 641b 9c02 641c 641d 8404 5a17 641e  d.d...d.d...Z.d.
+00000150: 641a 641b 9c02 641f 6420 8404 5a18 6508  d.d...d.d ..Z.e.
+00000160: 6410 6506 a019 a100 1b00 6412 6506 a019  d.e.......d.e...
+00000170: a100 1b00 6414 6506 a019 a100 1b00 6416  ....d.e.......d.
+00000180: 6506 a019 a100 1b00 6418 6506 a019 a100  e.......d.e.....
+00000190: 1b00 8305 5a1a 6402 5300 2921 e900 0000  ....Z.d.S.)!....
+000001a0: 0029 01da 0b61 6e6e 6f74 6174 696f 6e73  .)...annotations
+000001b0: 4e29 01da 0964 6174 6163 6c61 7373 2901  N)...dataclass).
+000001c0: da0e 456e 756d 466f 7243 6f64 6567 656e  ..EnumForCodegen
+000001d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000001e0: 0003 0000 0040 0000 0173 1600 0000 6500  .....@...s....e.
+000001f0: 5a01 6400 5a02 5500 6401 6503 6402 3c00  Z.d.Z.U.d.e.d.<.
+00000200: 6403 5300 2904 da11 556e 696e 6974 6961  d.S.)...Uninitia
+00000210: 6c69 7a65 644a 534f 4e7a 1f74 7970 696e  lizedJSONz.typin
+00000220: 672e 4c69 7465 7261 6c5b 2755 6e69 6e69  g.Literal['Unini
+00000230: 7469 616c 697a 6564 275d da04 6b69 6e64  tialized']..kind
+00000240: 4ea9 04da 085f 5f6e 616d 655f 5fda 0a5f  N....__name__.._
+00000250: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000260: 6c6e 616d 655f 5fda 0f5f 5f61 6e6e 6f74  lname__..__annot
+00000270: 6174 696f 6e73 5f5f a900 720c 0000 0072  ations__..r....r
+00000280: 0c00 0000 fa47 2f55 7365 7273 2f74 6672  .....G/Users/tfr
+00000290: 697a 7a61 2f44 6f63 756d 656e 7473 2f7a  izza/Documents/z
+000002a0: 6574 612f 7a65 7461 2d70 792f 7a65 7461  eta/zeta-py/zeta
+000002b0: 5f70 792f 7a65 7461 5f63 6c69 656e 742f  _py/zeta_client/
+000002c0: 7479 7065 732f 6b69 6e64 2e70 7972 0500  types/kind.pyr..
+000002d0: 0000 0a00 0000 7302 0000 000a 0172 0500  ......s......r..
+000002e0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000002f0: 0000 0003 0000 0040 0000 0173 1600 0000  .......@...s....
+00000300: 6500 5a01 6400 5a02 5500 6401 6503 6402  e.Z.d.Z.U.d.e.d.
+00000310: 3c00 6403 5300 2904 da08 4361 6c6c 4a53  <.d.S.)...CallJS
+00000320: 4f4e 7a16 7479 7069 6e67 2e4c 6974 6572  ONz.typing.Liter
+00000330: 616c 5b27 4361 6c6c 275d 7206 0000 004e  al['Call']r....N
+00000340: 7207 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+00000350: 0c00 0000 720d 0000 0072 0e00 0000 0e00  ....r....r......
+00000360: 0000 7302 0000 000a 0172 0e00 0000 6300  ..s......r....c.
+00000370: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000380: 0000 0040 0000 0173 1600 0000 6500 5a01  ...@...s....e.Z.
+00000390: 6400 5a02 5500 6401 6503 6402 3c00 6403  d.Z.U.d.e.d.<.d.
+000003a0: 5300 2904 da07 5075 744a 534f 4e7a 1574  S.)...PutJSONz.t
+000003b0: 7970 696e 672e 4c69 7465 7261 6c5b 2750  yping.Literal['P
+000003c0: 7574 275d 7206 0000 004e 7207 0000 0072  ut']r....Nr....r
+000003d0: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
+000003e0: 0000 0072 0f00 0000 1200 0000 7302 0000  ...r........s...
+000003f0: 000a 0172 0f00 0000 6300 0000 0000 0000  ...r....c.......
+00000400: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000410: 0173 1600 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
+00000420: 6401 6503 6402 3c00 6403 5300 2904 da0a  d.e.d.<.d.S.)...
+00000430: 4675 7475 7265 4a53 4f4e 7a18 7479 7069  FutureJSONz.typi
+00000440: 6e67 2e4c 6974 6572 616c 5b27 4675 7475  ng.Literal['Futu
+00000450: 7265 275d 7206 0000 004e 7207 0000 0072  re']r....Nr....r
+00000460: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
+00000470: 0000 0072 1000 0000 1600 0000 7302 0000  ...r........s...
+00000480: 000a 0172 1000 0000 6300 0000 0000 0000  ...r....c.......
+00000490: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+000004a0: 0173 1600 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
+000004b0: 6401 6503 6402 3c00 6403 5300 2904 da08  d.e.d.<.d.S.)...
+000004c0: 5065 7270 4a53 4f4e 7a16 7479 7069 6e67  PerpJSONz.typing
+000004d0: 2e4c 6974 6572 616c 5b27 5065 7270 275d  .Literal['Perp']
+000004e0: 7206 0000 004e 7207 0000 0072 0c00 0000  r....Nr....r....
+000004f0: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+00000500: 1100 0000 1a00 0000 7302 0000 000a 0172  ........s......r
+00000510: 1100 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000520: 0000 0000 0004 0000 0040 0000 0173 4a00  .........@...sJ.
+00000530: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
+00000540: 6402 6504 6403 3c00 6400 5a05 6402 6504  d.e.d.<.d.Z.d.e.
+00000550: 6404 3c00 6506 6405 6406 9c01 6407 6408  d.<.e.d.d...d.d.
+00000560: 8404 8301 5a07 6506 6409 6406 9c01 640a  ....Z.e.d.d...d.
+00000570: 640b 8404 8301 5a08 640c 5300 290d da0d  d.....Z.d.S.)...
+00000580: 556e 696e 6974 6961 6c69 7a65 6472 0100  Uninitializedr..
+00000590: 0000 fa0f 7479 7069 6e67 2e43 6c61 7373  ....typing.Class
+000005a0: 5661 72da 0d64 6973 6372 696d 696e 6174  Var..discriminat
+000005b0: 6f72 7206 0000 0072 0500 0000 a901 da06  orr....r........
+000005c0: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
+000005d0: 0000 0001 0000 0003 0000 0043 0000 0173  ...........C...s
+000005e0: 0a00 0000 7400 6401 6402 8d01 5300 2903  ....t.d.d...S.).
+000005f0: 4e72 1200 0000 a901 7206 0000 0029 0172  Nr......r....).r
+00000600: 0500 0000 a901 da03 636c 7372 0c00 0000  ........clsr....
+00000610: 720c 0000 0072 0d00 0000 da07 746f 5f6a  r....r......to_j
+00000620: 736f 6e23 0000 0073 0600 0000 0002 0201  son#...s........
+00000630: 02ff 7a15 556e 696e 6974 6961 6c69 7a65  ..z.Uninitialize
+00000640: 642e 746f 5f6a 736f 6eda 0464 6963 7463  d.to_json..dictc
+00000650: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000660: 0200 0000 4300 0001 7308 0000 0064 0169  ....C...s....d.i
+00000670: 0069 0153 0029 024e 7212 0000 0072 0c00  .i.S.).Nr....r..
+00000680: 0000 7218 0000 0072 0c00 0000 720c 0000  ..r....r....r...
+00000690: 0072 0d00 0000 da0c 746f 5f65 6e63 6f64  .r......to_encod
+000006a0: 6162 6c65 2900 0000 7304 0000 0000 0304  able)...s.......
+000006b0: ff7a 1a55 6e69 6e69 7469 616c 697a 6564  .z.Uninitialized
+000006c0: 2e74 6f5f 656e 636f 6461 626c 654e a909  .to_encodableN..
+000006d0: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+000006e0: 1400 0000 720b 0000 0072 0600 0000 da0b  ....r....r......
+000006f0: 636c 6173 736d 6574 686f 6472 1a00 0000  classmethodr....
+00000700: 721c 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+00000710: 0c00 0000 720d 0000 0072 1200 0000 1e00  ....r....r......
+00000720: 0000 730c 0000 000a 020c 010c 0202 0110  ..s.............
+00000730: 0502 0172 1200 0000 6300 0000 0000 0000  ...r....c.......
+00000740: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
+00000750: 0173 4a00 0000 6500 5a01 6400 5a02 5500  .sJ...e.Z.d.Z.U.
+00000760: 6401 5a03 6402 6504 6403 3c00 6400 5a05  d.Z.d.e.d.<.d.Z.
+00000770: 6402 6504 6404 3c00 6506 6405 6406 9c01  d.e.d.<.e.d.d...
+00000780: 6407 6408 8404 8301 5a07 6506 6409 6406  d.d.....Z.e.d.d.
+00000790: 9c01 640a 640b 8404 8301 5a08 640c 5300  ..d.d.....Z.d.S.
+000007a0: 290d da04 4361 6c6c e901 0000 0072 1300  )...Call.....r..
+000007b0: 0000 7214 0000 0072 0600 0000 720e 0000  ..r....r....r...
+000007c0: 0072 1500 0000 6301 0000 0000 0000 0000  .r....c.........
+000007d0: 0000 0001 0000 0003 0000 0043 0000 0173  ...........C...s
+000007e0: 0a00 0000 7400 6401 6402 8d01 5300 2903  ....t.d.d...S.).
+000007f0: 4e72 1f00 0000 7217 0000 0029 0172 0e00  Nr....r....).r..
+00000800: 0000 7218 0000 0072 0c00 0000 720c 0000  ..r....r....r...
+00000810: 0072 0d00 0000 721a 0000 0035 0000 0073  .r....r....5...s
+00000820: 0600 0000 0002 0201 02ff 7a0c 4361 6c6c  ..........z.Call
+00000830: 2e74 6f5f 6a73 6f6e 721b 0000 0063 0100  .to_jsonr....c..
+00000840: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00000850: 0000 4300 0001 7308 0000 0064 0169 0069  ..C...s....d.i.i
+00000860: 0153 0029 024e 721f 0000 0072 0c00 0000  .S.).Nr....r....
+00000870: 7218 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+00000880: 0d00 0000 721c 0000 003b 0000 0073 0400  ....r....;...s..
+00000890: 0000 0003 04ff 7a11 4361 6c6c 2e74 6f5f  ......z.Call.to_
+000008a0: 656e 636f 6461 626c 654e 721d 0000 0072  encodableNr....r
+000008b0: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
+000008c0: 0000 0072 1f00 0000 3000 0000 730c 0000  ...r....0...s...
+000008d0: 000a 020c 010c 0202 0110 0502 0172 1f00  .............r..
+000008e0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000008f0: 0000 0004 0000 0040 0000 0173 4a00 0000  .......@...sJ...
+00000900: 6500 5a01 6400 5a02 5500 6401 5a03 6402  e.Z.d.Z.U.d.Z.d.
+00000910: 6504 6403 3c00 6400 5a05 6402 6504 6404  e.d.<.d.Z.d.e.d.
+00000920: 3c00 6506 6405 6406 9c01 6407 6408 8404  <.e.d.d...d.d...
+00000930: 8301 5a07 6506 6409 6406 9c01 640a 640b  ..Z.e.d.d...d.d.
+00000940: 8404 8301 5a08 640c 5300 290d da03 5075  ....Z.d.S.)...Pu
+00000950: 74e9 0200 0000 7213 0000 0072 1400 0000  t.....r....r....
+00000960: 7206 0000 0072 0f00 0000 7215 0000 0063  r....r....r....c
+00000970: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000980: 0300 0000 4300 0001 730a 0000 0074 0064  ....C...s....t.d
+00000990: 0164 028d 0153 0029 034e 7221 0000 0072  .d...S.).Nr!...r
+000009a0: 1700 0000 2901 720f 0000 0072 1800 0000  ....).r....r....
+000009b0: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+000009c0: 1a00 0000 4700 0000 7306 0000 0000 0202  ....G...s.......
+000009d0: 0102 ff7a 0b50 7574 2e74 6f5f 6a73 6f6e  ...z.Put.to_json
+000009e0: 721b 0000 0063 0100 0000 0000 0000 0000  r....c..........
+000009f0: 0000 0100 0000 0200 0000 4300 0001 7308  ..........C...s.
+00000a00: 0000 0064 0169 0069 0153 0029 024e 7221  ...d.i.i.S.).Nr!
+00000a10: 0000 0072 0c00 0000 7218 0000 0072 0c00  ...r....r....r..
+00000a20: 0000 720c 0000 0072 0d00 0000 721c 0000  ..r....r....r...
+00000a30: 004d 0000 0073 0400 0000 0003 04ff 7a10  .M...s........z.
+00000a40: 5075 742e 746f 5f65 6e63 6f64 6162 6c65  Put.to_encodable
+00000a50: 4e72 1d00 0000 720c 0000 0072 0c00 0000  Nr....r....r....
+00000a60: 720c 0000 0072 0d00 0000 7221 0000 0042  r....r....r!...B
+00000a70: 0000 0073 0c00 0000 0a02 0c01 0c02 0201  ...s............
+00000a80: 1005 0201 7221 0000 0063 0000 0000 0000  ....r!...c......
+00000a90: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
+00000aa0: 0001 734a 0000 0065 005a 0164 005a 0255  ..sJ...e.Z.d.Z.U
+00000ab0: 0064 015a 0364 0265 0464 033c 0064 005a  .d.Z.d.e.d.<.d.Z
+00000ac0: 0564 0265 0464 043c 0065 0664 0564 069c  .d.e.d.<.e.d.d..
+00000ad0: 0164 0764 0884 0483 015a 0765 0664 0964  .d.d.....Z.e.d.d
+00000ae0: 069c 0164 0a64 0b84 0483 015a 0864 0c53  ...d.d.....Z.d.S
+00000af0: 0029 0dda 0646 7574 7572 65e9 0300 0000  .)...Future.....
+00000b00: 7213 0000 0072 1400 0000 7206 0000 0072  r....r....r....r
+00000b10: 1000 0000 7215 0000 0063 0100 0000 0000  ....r....c......
+00000b20: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00000b30: 0001 730a 0000 0074 0064 0164 028d 0153  ..s....t.d.d...S
+00000b40: 0029 034e 7223 0000 0072 1700 0000 2901  .).Nr#...r....).
+00000b50: 7210 0000 0072 1800 0000 720c 0000 0072  r....r....r....r
+00000b60: 0c00 0000 720d 0000 0072 1a00 0000 5900  ....r....r....Y.
+00000b70: 0000 7306 0000 0000 0202 0102 ff7a 0e46  ..s..........z.F
+00000b80: 7574 7572 652e 746f 5f6a 736f 6e72 1b00  uture.to_jsonr..
+00000b90: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00000ba0: 0000 0002 0000 0043 0000 0173 0800 0000  .......C...s....
+00000bb0: 6401 6900 6901 5300 2902 4e72 2300 0000  d.i.i.S.).Nr#...
+00000bc0: 720c 0000 0072 1800 0000 720c 0000 0072  r....r....r....r
+00000bd0: 0c00 0000 720d 0000 0072 1c00 0000 5f00  ....r....r...._.
+00000be0: 0000 7304 0000 0000 0304 ff7a 1346 7574  ..s........z.Fut
+00000bf0: 7572 652e 746f 5f65 6e63 6f64 6162 6c65  ure.to_encodable
+00000c00: 4e72 1d00 0000 720c 0000 0072 0c00 0000  Nr....r....r....
+00000c10: 720c 0000 0072 0d00 0000 7223 0000 0054  r....r....r#...T
+00000c20: 0000 0073 0c00 0000 0a02 0c01 0c02 0201  ...s............
+00000c30: 1005 0201 7223 0000 0063 0000 0000 0000  ....r#...c......
+00000c40: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
+00000c50: 0001 734a 0000 0065 005a 0164 005a 0255  ..sJ...e.Z.d.Z.U
+00000c60: 0064 015a 0364 0265 0464 033c 0064 005a  .d.Z.d.e.d.<.d.Z
+00000c70: 0564 0265 0464 043c 0065 0664 0564 069c  .d.e.d.<.e.d.d..
+00000c80: 0164 0764 0884 0483 015a 0765 0664 0964  .d.d.....Z.e.d.d
+00000c90: 069c 0164 0a64 0b84 0483 015a 0864 0c53  ...d.d.....Z.d.S
+00000ca0: 0029 0dda 0450 6572 70e9 0400 0000 7213  .)...Perp.....r.
+00000cb0: 0000 0072 1400 0000 7206 0000 0072 1100  ...r....r....r..
+00000cc0: 0000 7215 0000 0063 0100 0000 0000 0000  ..r....c........
+00000cd0: 0000 0000 0100 0000 0300 0000 4300 0001  ............C...
+00000ce0: 730a 0000 0074 0064 0164 028d 0153 0029  s....t.d.d...S.)
+00000cf0: 034e 7225 0000 0072 1700 0000 2901 7211  .Nr%...r....).r.
+00000d00: 0000 0072 1800 0000 720c 0000 0072 0c00  ...r....r....r..
+00000d10: 0000 720d 0000 0072 1a00 0000 6b00 0000  ..r....r....k...
+00000d20: 7306 0000 0000 0202 0102 ff7a 0c50 6572  s..........z.Per
+00000d30: 702e 746f 5f6a 736f 6e72 1b00 0000 6301  p.to_jsonr....c.
+00000d40: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00000d50: 0000 0043 0000 0173 0800 0000 6401 6900  ...C...s....d.i.
+00000d60: 6901 5300 2902 4e72 2500 0000 720c 0000  i.S.).Nr%...r...
+00000d70: 0072 1800 0000 720c 0000 0072 0c00 0000  .r....r....r....
+00000d80: 720d 0000 0072 1c00 0000 7100 0000 7304  r....r....q...s.
+00000d90: 0000 0000 0304 ff7a 1150 6572 702e 746f  .......z.Perp.to
+00000da0: 5f65 6e63 6f64 6162 6c65 4e72 1d00 0000  _encodableNr....
+00000db0: 720c 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+00000dc0: 0d00 0000 7225 0000 0066 0000 0073 0c00  ....r%...f...s..
+00000dd0: 0000 0a02 0c01 0c02 0201 1005 0201 7225  ..............r%
+00000de0: 0000 0072 1b00 0000 da08 4b69 6e64 4b69  ...r......KindKi
+00000df0: 6e64 2902 da03 6f62 6a72 1600 0000 6301  nd)...objr....c.
+00000e00: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00000e10: 0000 0043 0000 0173 6400 0000 7400 7c00  ...C...sd...t.|.
+00000e20: 7401 8302 7312 7402 6401 8301 8201 6402  t...s.t.d.....d.
+00000e30: 7c00 7600 7220 7403 8300 5300 6403 7c00  |.v.r t...S.d.|.
+00000e40: 7600 722e 7404 8300 5300 6404 7c00 7600  v.r.t...S.d.|.v.
+00000e50: 723c 7405 8300 5300 6405 7c00 7600 724a  r<t...S.d.|.v.rJ
+00000e60: 7406 8300 5300 6406 7c00 7600 7258 7407  t...S.d.|.v.rXt.
+00000e70: 8300 5300 7402 6401 8301 8201 6400 5300  ..S.t.d.....d.S.
+00000e80: 2907 4e7a 1349 6e76 616c 6964 2065 6e75  ).Nz.Invalid enu
+00000e90: 6d20 6f62 6a65 6374 7212 0000 0072 1f00  m objectr....r..
+00000ea0: 0000 7221 0000 0072 2300 0000 7225 0000  ..r!...r#...r%..
+00000eb0: 0029 08da 0a69 7369 6e73 7461 6e63 6572  .)...isinstancer
+00000ec0: 1b00 0000 da0a 5661 6c75 6545 7272 6f72  ......ValueError
+00000ed0: 7212 0000 0072 1f00 0000 7221 0000 0072  r....r....r!...r
+00000ee0: 2300 0000 7225 0000 0029 0172 2800 0000  #...r%...).r(...
+00000ef0: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+00000f00: 0c66 726f 6d5f 6465 636f 6465 647c 0000  .from_decoded|..
+00000f10: 0073 1a00 0000 0001 0a01 0801 0801 0601  .s..............
+00000f20: 0801 0601 0801 0601 0801 0601 0801 0601  ................
+00000f30: 722b 0000 00da 084b 696e 644a 534f 4e63  r+.....KindJSONc
+00000f40: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000f50: 0300 0000 4300 0001 7374 0000 007c 0064  ....C...st...|.d
+00000f60: 0119 0064 026b 0272 1274 0083 0053 007c  ...d.k.r.t...S.|
+00000f70: 0064 0119 0064 036b 0272 2474 0183 0053  .d...d.k.r$t...S
+00000f80: 007c 0064 0119 0064 046b 0272 3674 0283  .|.d...d.k.r6t..
+00000f90: 0053 007c 0064 0119 0064 056b 0272 4874  .S.|.d...d.k.rHt
+00000fa0: 0383 0053 007c 0064 0119 0064 066b 0272  ...S.|.d...d.k.r
+00000fb0: 5a74 0483 0053 007c 0064 0119 007d 0174  Zt...S.|.d...}.t
+00000fc0: 0564 077c 019b 009d 0283 0182 0164 0053  .d.|.........d.S
+00000fd0: 0029 084e 7206 0000 0072 1200 0000 721f  .).Nr....r....r.
+00000fe0: 0000 0072 2100 0000 7223 0000 0072 2500  ...r!...r#...r%.
+00000ff0: 0000 7a18 556e 7265 636f 676e 697a 6564  ..z.Unrecognized
+00001000: 2065 6e75 6d20 6b69 6e64 3a20 2906 7212   enum kind: ).r.
+00001010: 0000 0072 1f00 0000 7221 0000 0072 2300  ...r....r!...r#.
+00001020: 0000 7225 0000 0072 2a00 0000 2902 7228  ..r%...r*...).r(
+00001030: 0000 0072 0600 0000 720c 0000 0072 0c00  ...r....r....r..
+00001040: 0000 720d 0000 00da 0966 726f 6d5f 6a73  ..r......from_js
+00001050: 6f6e 8c00 0000 7318 0000 0000 010c 0106  on....s.........
+00001060: 010c 0106 010c 0106 010c 0106 010c 0106  ................
+00001070: 0108 0172 2d00 0000 291b da0a 5f5f 6675  ...r-...)...__fu
+00001080: 7475 7265 5f5f 7202 0000 00da 0674 7970  ture__r......typ
+00001090: 696e 67da 0b64 6174 6163 6c61 7373 6573  ing..dataclasses
+000010a0: 7203 0000 00da 0f62 6f72 7368 5f63 6f6e  r......borsh_con
+000010b0: 7374 7275 6374 da05 626f 7273 68da 1861  struct..borsh..a
+000010c0: 6e63 686f 7270 792e 626f 7273 685f 6578  nchorpy.borsh_ex
+000010d0: 7465 6e73 696f 6e72 0400 0000 da09 5479  tensionr......Ty
+000010e0: 7065 6444 6963 7472 0500 0000 720e 0000  pedDictr....r...
+000010f0: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
+00001100: 7212 0000 0072 1f00 0000 7221 0000 0072  r....r....r!...r
+00001110: 2300 0000 7225 0000 00da 0555 6e69 6f6e  #...r%.....Union
+00001120: 7227 0000 0072 2c00 0000 722b 0000 0072  r'...r,...r+...r
+00001130: 2d00 0000 da07 4353 7472 7563 74da 066c  -.....CStruct..l
+00001140: 6179 6f75 7472 0c00 0000 720c 0000 0072  ayoutr....r....r
+00001150: 0c00 0000 720d 0000 00da 083c 6d6f 6475  ....r......<modu
+00001160: 6c65 3e01 0000 0073 3c00 0000 0c02 0801  le>....s<.......
+00001170: 0c02 0801 0c03 1204 1204 1204 1204 1204  ................
+00001180: 0201 1011 0201 1011 0201 1011 0201 1011  ................
+00001190: 0201 1011 1401 1403 1010 100f 0201 0a01  ................
+000011a0: 0a01 0a01 0a01 0afb                      ........
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/cross_margin_account_info.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/cross_margin_account_info.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/cross_margin_account_info.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/cross_margin_account_info.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/expire_series_override_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/expire_series_override_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/expire_series_override_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/expire_series_override_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/expiry_series.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/expiry_series.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/expiry_series.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/expiry_series.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/expiry_series_status.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/expiry_series_status.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/expiry_series_status.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/expiry_series_status.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/halt_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/halt_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/halt_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/halt_args.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Aug 21 13:18:23 2023 UTC, .py size: 961 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1f64 e364 c103 0000  a........d.d....
+00000000: 610d 0d0a 0000 0000 ae9a 6865 c103 0000  a.........he....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6402 6c05 5a06 6400 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6502 6a09  ..G.d.d...d.e.j.
 00000070: 8303 5a0a 6504 4700 6407 6408 8400 6408  ..Z.e.G.d.d...d.
@@ -17,83 +17,84 @@
 00000100: 7267 734a 534f 4efa 096c 6973 745b 696e  rgsJSON..list[in
 00000110: 745d da0b 7370 6f74 5f70 7269 6365 73da  t]..spot_prices.
 00000120: 0369 6e74 da09 7469 6d65 7374 616d 704e  .int..timestampN
 00000130: 2904 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 00000140: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 00000150: 6e61 6d65 5f5f da0f 5f5f 616e 6e6f 7461  name__..__annota
 00000160: 7469 6f6e 735f 5fa9 0072 0e00 0000 720e  tions__..r....r.
-00000170: 0000 00fa 4c2f 5573 6572 732f 7466 7269  ....L/Users/tfri
+00000170: 0000 00fa 5a2f 5573 6572 732f 7466 7269  ....Z/Users/tfri
 00000180: 7a7a 612f 446f 6375 6d65 6e74 732f 7a65  zza/Documents/ze
-00000190: 7461 2f7a 6574 612d 7079 2f7a 6574 615f  ta/zeta-py/zeta_
-000001a0: 7079 2f7a 6574 615f 636c 6965 6e74 2f74  py/zeta_client/t
-000001b0: 7970 6573 2f68 616c 745f 6172 6773 2e70  ypes/halt_args.p
-000001c0: 7972 0500 0000 0a00 0000 7304 0000 000a  yr........s.....
-000001d0: 0108 0172 0500 0000 6300 0000 0000 0000  ...r....c.......
-000001e0: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
-000001f0: 0173 8600 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
-00000200: 6503 a004 6401 6503 6a05 6402 1900 1b00  e...d.e.j.d.....
-00000210: 6403 6503 6a05 1b00 a102 5a06 6404 6507  d.e.j.....Z.d.e.
-00000220: 6405 3c00 6406 6507 6401 3c00 6407 6507  d.<.d.e.d.<.d.e.
-00000230: 6403 3c00 6508 6408 6409 640a 9c02 640b  d.<.e.d.d.d...d.
-00000240: 640c 8404 8301 5a09 640d 640e 9c01 640f  d.....Z.d.d...d.
-00000250: 6410 8404 5a0a 6411 640e 9c01 6412 6413  d...Z.d.d...d.d.
-00000260: 8404 5a0b 6508 6411 6409 640a 9c02 6414  ..Z.e.d.d.d...d.
-00000270: 6415 8404 8301 5a0c 6416 5300 2917 da08  d.....Z.d.S.)...
-00000280: 4861 6c74 4172 6773 7207 0000 00e9 0500  HaltArgsr.......
-00000290: 0000 7209 0000 007a 0f74 7970 696e 672e  ..r....z.typing.
-000002a0: 436c 6173 7356 6172 da06 6c61 796f 7574  ClassVar..layout
-000002b0: 7206 0000 0072 0800 0000 7204 0000 007a  r....r....r....z
-000002c0: 0a27 4861 6c74 4172 6773 2729 02da 036f  .'HaltArgs')...o
-000002d0: 626a da06 7265 7475 726e 6302 0000 0000  bj..returnc.....
-000002e0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-000002f0: 0000 0173 1000 0000 7c00 7c01 6a00 7c01  ...s....|.|.j.|.
-00000300: 6a01 6401 8d02 5300 a902 4ea9 0272 0700  j.d...S...N..r..
-00000310: 0000 7209 0000 0072 1600 0000 a902 da03  ..r....r........
-00000320: 636c 7372 1300 0000 720e 0000 0072 0e00  clsr....r....r..
-00000330: 0000 720f 0000 00da 0c66 726f 6d5f 6465  ..r......from_de
-00000340: 636f 6465 6415 0000 0073 0200 0000 0002  coded....s......
-00000350: 7a15 4861 6c74 4172 6773 2e66 726f 6d5f  z.HaltArgs.from_
-00000360: 6465 636f 6465 647a 1564 6963 745b 7374  decodedz.dict[st
-00000370: 722c 2074 7970 696e 672e 416e 795d 2901  r, typing.Any]).
-00000380: 7214 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00000390: 0000 0100 0000 0300 0000 4300 0001 730e  ..........C...s.
-000003a0: 0000 007c 006a 007c 006a 0164 019c 0253  ...|.j.|.j.d...S
-000003b0: 0072 1500 0000 7216 0000 00a9 01da 0473  .r....r........s
-000003c0: 656c 6672 0e00 0000 720e 0000 0072 0f00  elfr....r....r..
-000003d0: 0000 da0c 746f 5f65 6e63 6f64 6162 6c65  ....to_encodable
-000003e0: 1900 0000 7302 0000 0000 017a 1548 616c  ....s......z.Hal
-000003f0: 7441 7267 732e 746f 5f65 6e63 6f64 6162  tArgs.to_encodab
-00000400: 6c65 7205 0000 0063 0100 0000 0000 0000  ler....c........
-00000410: 0000 0000 0100 0000 0300 0000 4300 0001  ............C...
-00000420: 730e 0000 007c 006a 007c 006a 0164 019c  s....|.j.|.j.d..
-00000430: 0253 0072 1500 0000 7216 0000 0072 1a00  .S.r....r....r..
-00000440: 0000 720e 0000 0072 0e00 0000 720f 0000  ..r....r....r...
-00000450: 00da 0774 6f5f 6a73 6f6e 1c00 0000 7302  ...to_json....s.
-00000460: 0000 0000 017a 1048 616c 7441 7267 732e  .....z.HaltArgs.
-00000470: 746f 5f6a 736f 6e63 0200 0000 0000 0000  to_jsonc........
-00000480: 0000 0000 0200 0000 0400 0000 4300 0001  ............C...
-00000490: 7314 0000 007c 007c 0164 0119 007c 0164  s....|.|.d...|.d
-000004a0: 0219 0064 038d 0253 0029 044e 7207 0000  ...d...S.).Nr...
-000004b0: 0072 0900 0000 7216 0000 0072 0e00 0000  .r....r....r....
-000004c0: 7217 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
-000004d0: 0f00 0000 da09 6672 6f6d 5f6a 736f 6e1f  ......from_json.
-000004e0: 0000 0073 0200 0000 0002 7a12 4861 6c74  ...s......z.Halt
-000004f0: 4172 6773 2e66 726f 6d5f 6a73 6f6e 4e29  Args.from_jsonN)
-00000500: 0d72 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00000510: da05 626f 7273 68da 0743 5374 7275 6374  ..borsh..CStruct
-00000520: da03 5536 3472 1200 0000 720d 0000 00da  ..U64r....r.....
-00000530: 0b63 6c61 7373 6d65 7468 6f64 7219 0000  .classmethodr...
-00000540: 0072 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
-00000550: 720e 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
-00000560: 0f00 0000 7210 0000 000f 0000 0073 1200  ....r........s..
-00000570: 0000 0a02 2401 0801 0802 0201 1203 0e03  ....$...........
-00000580: 0e03 0201 7210 0000 0029 0cda 0a5f 5f66  ....r....)...__f
-00000590: 7574 7572 655f 5f72 0200 0000 da06 7479  uture__r......ty
-000005a0: 7069 6e67 da0b 6461 7461 636c 6173 7365  ping..dataclasse
-000005b0: 7372 0300 0000 da0f 626f 7273 685f 636f  sr......borsh_co
-000005c0: 6e73 7472 7563 7472 1f00 0000 da09 636f  nstructr......co
-000005d0: 6e73 7472 7563 7472 0400 0000 da09 5479  nstructr......Ty
-000005e0: 7065 6444 6963 7472 0500 0000 7210 0000  pedDictr....r...
-000005f0: 0072 0e00 0000 720e 0000 0072 0e00 0000  .r....r....r....
-00000600: 720f 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000610: 0000 0073 0e00 0000 0c02 0801 0c02 0801  ...s............
-00000620: 0c03 1205 0201                           ......
+00000190: 7461 2f7a 6574 616d 6172 6b65 7473 2d70  ta/zetamarkets-p
+000001a0: 792f 7a65 7461 6d61 726b 6574 735f 7079  y/zetamarkets_py
+000001b0: 2f7a 6574 615f 636c 6965 6e74 2f74 7970  /zeta_client/typ
+000001c0: 6573 2f68 616c 745f 6172 6773 2e70 7972  es/halt_args.pyr
+000001d0: 0500 0000 0a00 0000 7304 0000 000a 0108  ........s.......
+000001e0: 0172 0500 0000 6300 0000 0000 0000 0000  .r....c.........
+000001f0: 0000 0000 0000 0005 0000 0040 0000 0173  ...........@...s
+00000200: 8600 0000 6500 5a01 6400 5a02 5500 6503  ....e.Z.d.Z.U.e.
+00000210: a004 6401 6503 6a05 6402 1900 1b00 6403  ..d.e.j.d.....d.
+00000220: 6503 6a05 1b00 a102 5a06 6404 6507 6405  e.j.....Z.d.e.d.
+00000230: 3c00 6406 6507 6401 3c00 6407 6507 6403  <.d.e.d.<.d.e.d.
+00000240: 3c00 6508 6408 6409 640a 9c02 640b 640c  <.e.d.d.d...d.d.
+00000250: 8404 8301 5a09 640d 640e 9c01 640f 6410  ....Z.d.d...d.d.
+00000260: 8404 5a0a 6411 640e 9c01 6412 6413 8404  ..Z.d.d...d.d...
+00000270: 5a0b 6508 6411 6409 640a 9c02 6414 6415  Z.e.d.d.d...d.d.
+00000280: 8404 8301 5a0c 6416 5300 2917 da08 4861  ....Z.d.S.)...Ha
+00000290: 6c74 4172 6773 7207 0000 00e9 0700 0000  ltArgsr.........
+000002a0: 7209 0000 007a 0f74 7970 696e 672e 436c  r....z.typing.Cl
+000002b0: 6173 7356 6172 da06 6c61 796f 7574 7206  assVar..layoutr.
+000002c0: 0000 0072 0800 0000 7204 0000 007a 0a27  ...r....r....z.'
+000002d0: 4861 6c74 4172 6773 2729 02da 036f 626a  HaltArgs')...obj
+000002e0: da06 7265 7475 726e 6302 0000 0000 0000  ..returnc.......
+000002f0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00000300: 0173 1000 0000 7c00 7c01 6a00 7c01 6a01  .s....|.|.j.|.j.
+00000310: 6401 8d02 5300 a902 4ea9 0272 0700 0000  d...S...N..r....
+00000320: 7209 0000 0072 1600 0000 a902 da03 636c  r....r........cl
+00000330: 7372 1300 0000 720e 0000 0072 0e00 0000  sr....r....r....
+00000340: 720f 0000 00da 0c66 726f 6d5f 6465 636f  r......from_deco
+00000350: 6465 6415 0000 0073 0200 0000 0002 7a15  ded....s......z.
+00000360: 4861 6c74 4172 6773 2e66 726f 6d5f 6465  HaltArgs.from_de
+00000370: 636f 6465 647a 1564 6963 745b 7374 722c  codedz.dict[str,
+00000380: 2074 7970 696e 672e 416e 795d 2901 7214   typing.Any]).r.
+00000390: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+000003a0: 0100 0000 0300 0000 4300 0001 730e 0000  ........C...s...
+000003b0: 007c 006a 007c 006a 0164 019c 0253 0072  .|.j.|.j.d...S.r
+000003c0: 1500 0000 7216 0000 00a9 01da 0473 656c  ....r........sel
+000003d0: 6672 0e00 0000 720e 0000 0072 0f00 0000  fr....r....r....
+000003e0: da0c 746f 5f65 6e63 6f64 6162 6c65 1900  ..to_encodable..
+000003f0: 0000 7302 0000 0000 017a 1548 616c 7441  ..s......z.HaltA
+00000400: 7267 732e 746f 5f65 6e63 6f64 6162 6c65  rgs.to_encodable
+00000410: 7205 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00000420: 0000 0100 0000 0300 0000 4300 0001 730e  ..........C...s.
+00000430: 0000 007c 006a 007c 006a 0164 019c 0253  ...|.j.|.j.d...S
+00000440: 0072 1500 0000 7216 0000 0072 1a00 0000  .r....r....r....
+00000450: 720e 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
+00000460: 0774 6f5f 6a73 6f6e 1c00 0000 7302 0000  .to_json....s...
+00000470: 0000 017a 1048 616c 7441 7267 732e 746f  ...z.HaltArgs.to
+00000480: 5f6a 736f 6e63 0200 0000 0000 0000 0000  _jsonc..........
+00000490: 0000 0200 0000 0400 0000 4300 0001 7314  ..........C...s.
+000004a0: 0000 007c 007c 0164 0119 007c 0164 0219  ...|.|.d...|.d..
+000004b0: 0064 038d 0253 0029 044e 7207 0000 0072  .d...S.).Nr....r
+000004c0: 0900 0000 7216 0000 0072 0e00 0000 7217  ....r....r....r.
+000004d0: 0000 0072 0e00 0000 720e 0000 0072 0f00  ...r....r....r..
+000004e0: 0000 da09 6672 6f6d 5f6a 736f 6e1f 0000  ....from_json...
+000004f0: 0073 0200 0000 0002 7a12 4861 6c74 4172  .s......z.HaltAr
+00000500: 6773 2e66 726f 6d5f 6a73 6f6e 4e29 0d72  gs.from_jsonN).r
+00000510: 0a00 0000 720b 0000 0072 0c00 0000 da05  ....r....r......
+00000520: 626f 7273 68da 0743 5374 7275 6374 da03  borsh..CStruct..
+00000530: 5536 3472 1200 0000 720d 0000 00da 0b63  U64r....r......c
+00000540: 6c61 7373 6d65 7468 6f64 7219 0000 0072  lassmethodr....r
+00000550: 1c00 0000 721d 0000 0072 1e00 0000 720e  ....r....r....r.
+00000560: 0000 0072 0e00 0000 720e 0000 0072 0f00  ...r....r....r..
+00000570: 0000 7210 0000 000f 0000 0073 1200 0000  ..r........s....
+00000580: 0a02 2401 0801 0802 0201 1203 0e03 0e03  ..$.............
+00000590: 0201 7210 0000 0029 0cda 0a5f 5f66 7574  ..r....)...__fut
+000005a0: 7572 655f 5f72 0200 0000 da06 7479 7069  ure__r......typi
+000005b0: 6e67 da0b 6461 7461 636c 6173 7365 7372  ng..dataclassesr
+000005c0: 0300 0000 da0f 626f 7273 685f 636f 6e73  ......borsh_cons
+000005d0: 7472 7563 7472 1f00 0000 da09 636f 6e73  tructr......cons
+000005e0: 7472 7563 7472 0400 0000 da09 5479 7065  tructr......Type
+000005f0: 6444 6963 7472 0500 0000 7210 0000 0072  dDictr....r....r
+00000600: 0e00 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
+00000610: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000620: 0073 0e00 0000 0c02 0801 0c02 0801 0c03  .s..............
+00000630: 1205 0201                                ....
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/halt_state.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/halt_state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/halt_state.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/halt_state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/halt_state_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/halt_state_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/halt_state_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/halt_state_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/halt_state_v2.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/halt_state_v2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/halt_state_v2.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/halt_state_v2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_market_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_market_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_market_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_market_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_market_node_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_market_node_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_market_node_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_market_node_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_state_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_state_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_state_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_state_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_zeta_group_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_zeta_group_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_zeta_group_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_zeta_group_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_zeta_pricing_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_zeta_pricing_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/initialize_zeta_pricing_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/initialize_zeta_pricing_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/kind.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/kind.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/kind.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/order_type.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Aug 21 13:18:23 2023 UTC, .py size: 3320 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1f64 e364 f80c 0000  a........d.d....
+00000000: 610d 0d0a 0000 0000 1f64 e364 6a0e 0000  a........d.dj...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0173 6c01 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6402 6c05 5a06 6400 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6502 6a09  ..G.d.d...d.e.j.
 00000070: 8303 5a0a 4700 6407 6408 8400 6408 6502  ..Z.G.d.d...d.e.
@@ -26,258 +26,266 @@
 00000190: 1b00 8305 5a1a 6402 5300 2921 e900 0000  ....Z.d.S.)!....
 000001a0: 0029 01da 0b61 6e6e 6f74 6174 696f 6e73  .)...annotations
 000001b0: 4e29 01da 0964 6174 6163 6c61 7373 2901  N)...dataclass).
 000001c0: da0e 456e 756d 466f 7243 6f64 6567 656e  ..EnumForCodegen
 000001d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 000001e0: 0003 0000 0040 0000 0173 1600 0000 6500  .....@...s....e.
 000001f0: 5a01 6400 5a02 5500 6401 6503 6402 3c00  Z.d.Z.U.d.e.d.<.
-00000200: 6403 5300 2904 da11 556e 696e 6974 6961  d.S.)...Uninitia
-00000210: 6c69 7a65 644a 534f 4e7a 1f74 7970 696e  lizedJSONz.typin
-00000220: 672e 4c69 7465 7261 6c5b 2755 6e69 6e69  g.Literal['Unini
-00000230: 7469 616c 697a 6564 275d da04 6b69 6e64  tialized']..kind
-00000240: 4ea9 04da 085f 5f6e 616d 655f 5fda 0a5f  N....__name__.._
-00000250: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000260: 6c6e 616d 655f 5fda 0f5f 5f61 6e6e 6f74  lname__..__annot
-00000270: 6174 696f 6e73 5f5f a900 720c 0000 0072  ations__..r....r
-00000280: 0c00 0000 fa47 2f55 7365 7273 2f74 6672  .....G/Users/tfr
-00000290: 697a 7a61 2f44 6f63 756d 656e 7473 2f7a  izza/Documents/z
-000002a0: 6574 612f 7a65 7461 2d70 792f 7a65 7461  eta/zeta-py/zeta
-000002b0: 5f70 792f 7a65 7461 5f63 6c69 656e 742f  _py/zeta_client/
-000002c0: 7479 7065 732f 6b69 6e64 2e70 7972 0500  types/kind.pyr..
-000002d0: 0000 0a00 0000 7302 0000 000a 0172 0500  ......s......r..
-000002e0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000002f0: 0000 0003 0000 0040 0000 0173 1600 0000  .......@...s....
-00000300: 6500 5a01 6400 5a02 5500 6401 6503 6402  e.Z.d.Z.U.d.e.d.
-00000310: 3c00 6403 5300 2904 da08 4361 6c6c 4a53  <.d.S.)...CallJS
-00000320: 4f4e 7a16 7479 7069 6e67 2e4c 6974 6572  ONz.typing.Liter
-00000330: 616c 5b27 4361 6c6c 275d 7206 0000 004e  al['Call']r....N
-00000340: 7207 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
-00000350: 0c00 0000 720d 0000 0072 0e00 0000 0e00  ....r....r......
-00000360: 0000 7302 0000 000a 0172 0e00 0000 6300  ..s......r....c.
-00000370: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00000380: 0000 0040 0000 0173 1600 0000 6500 5a01  ...@...s....e.Z.
-00000390: 6400 5a02 5500 6401 6503 6402 3c00 6403  d.Z.U.d.e.d.<.d.
-000003a0: 5300 2904 da07 5075 744a 534f 4e7a 1574  S.)...PutJSONz.t
-000003b0: 7970 696e 672e 4c69 7465 7261 6c5b 2750  yping.Literal['P
-000003c0: 7574 275d 7206 0000 004e 7207 0000 0072  ut']r....Nr....r
-000003d0: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-000003e0: 0000 0072 0f00 0000 1200 0000 7302 0000  ...r........s...
-000003f0: 000a 0172 0f00 0000 6300 0000 0000 0000  ...r....c.......
-00000400: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000410: 0173 1600 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
-00000420: 6401 6503 6402 3c00 6403 5300 2904 da0a  d.e.d.<.d.S.)...
-00000430: 4675 7475 7265 4a53 4f4e 7a18 7479 7069  FutureJSONz.typi
-00000440: 6e67 2e4c 6974 6572 616c 5b27 4675 7475  ng.Literal['Futu
-00000450: 7265 275d 7206 0000 004e 7207 0000 0072  re']r....Nr....r
-00000460: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-00000470: 0000 0072 1000 0000 1600 0000 7302 0000  ...r........s...
-00000480: 000a 0172 1000 0000 6300 0000 0000 0000  ...r....c.......
-00000490: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-000004a0: 0173 1600 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
-000004b0: 6401 6503 6402 3c00 6403 5300 2904 da08  d.e.d.<.d.S.)...
-000004c0: 5065 7270 4a53 4f4e 7a16 7479 7069 6e67  PerpJSONz.typing
-000004d0: 2e4c 6974 6572 616c 5b27 5065 7270 275d  .Literal['Perp']
-000004e0: 7206 0000 004e 7207 0000 0072 0c00 0000  r....Nr....r....
-000004f0: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
-00000500: 1100 0000 1a00 0000 7302 0000 000a 0172  ........s......r
-00000510: 1100 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000520: 0000 0000 0004 0000 0040 0000 0173 4a00  .........@...sJ.
-00000530: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
-00000540: 6402 6504 6403 3c00 6400 5a05 6402 6504  d.e.d.<.d.Z.d.e.
-00000550: 6404 3c00 6506 6405 6406 9c01 6407 6408  d.<.e.d.d...d.d.
-00000560: 8404 8301 5a07 6506 6409 6406 9c01 640a  ....Z.e.d.d...d.
-00000570: 640b 8404 8301 5a08 640c 5300 290d da0d  d.....Z.d.S.)...
-00000580: 556e 696e 6974 6961 6c69 7a65 6472 0100  Uninitializedr..
-00000590: 0000 fa0f 7479 7069 6e67 2e43 6c61 7373  ....typing.Class
-000005a0: 5661 72da 0d64 6973 6372 696d 696e 6174  Var..discriminat
-000005b0: 6f72 7206 0000 0072 0500 0000 a901 da06  orr....r........
-000005c0: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
-000005d0: 0000 0001 0000 0003 0000 0043 0000 0173  ...........C...s
-000005e0: 0a00 0000 7400 6401 6402 8d01 5300 2903  ....t.d.d...S.).
-000005f0: 4e72 1200 0000 a901 7206 0000 0029 0172  Nr......r....).r
-00000600: 0500 0000 a901 da03 636c 7372 0c00 0000  ........clsr....
-00000610: 720c 0000 0072 0d00 0000 da07 746f 5f6a  r....r......to_j
-00000620: 736f 6e23 0000 0073 0600 0000 0002 0201  son#...s........
-00000630: 02ff 7a15 556e 696e 6974 6961 6c69 7a65  ..z.Uninitialize
-00000640: 642e 746f 5f6a 736f 6eda 0464 6963 7463  d.to_json..dictc
-00000650: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000660: 0200 0000 4300 0001 7308 0000 0064 0169  ....C...s....d.i
-00000670: 0069 0153 0029 024e 7212 0000 0072 0c00  .i.S.).Nr....r..
-00000680: 0000 7218 0000 0072 0c00 0000 720c 0000  ..r....r....r...
-00000690: 0072 0d00 0000 da0c 746f 5f65 6e63 6f64  .r......to_encod
-000006a0: 6162 6c65 2900 0000 7304 0000 0000 0304  able)...s.......
-000006b0: ff7a 1a55 6e69 6e69 7469 616c 697a 6564  .z.Uninitialized
-000006c0: 2e74 6f5f 656e 636f 6461 626c 654e a909  .to_encodableN..
-000006d0: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-000006e0: 1400 0000 720b 0000 0072 0600 0000 da0b  ....r....r......
-000006f0: 636c 6173 736d 6574 686f 6472 1a00 0000  classmethodr....
-00000700: 721c 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
-00000710: 0c00 0000 720d 0000 0072 1200 0000 1e00  ....r....r......
-00000720: 0000 730c 0000 000a 020c 010c 0202 0110  ..s.............
-00000730: 0502 0172 1200 0000 6300 0000 0000 0000  ...r....c.......
-00000740: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000750: 0173 4a00 0000 6500 5a01 6400 5a02 5500  .sJ...e.Z.d.Z.U.
-00000760: 6401 5a03 6402 6504 6403 3c00 6400 5a05  d.Z.d.e.d.<.d.Z.
-00000770: 6402 6504 6404 3c00 6506 6405 6406 9c01  d.e.d.<.e.d.d...
-00000780: 6407 6408 8404 8301 5a07 6506 6409 6406  d.d.....Z.e.d.d.
-00000790: 9c01 640a 640b 8404 8301 5a08 640c 5300  ..d.d.....Z.d.S.
-000007a0: 290d da04 4361 6c6c e901 0000 0072 1300  )...Call.....r..
-000007b0: 0000 7214 0000 0072 0600 0000 720e 0000  ..r....r....r...
-000007c0: 0072 1500 0000 6301 0000 0000 0000 0000  .r....c.........
-000007d0: 0000 0001 0000 0003 0000 0043 0000 0173  ...........C...s
-000007e0: 0a00 0000 7400 6401 6402 8d01 5300 2903  ....t.d.d...S.).
-000007f0: 4e72 1f00 0000 7217 0000 0029 0172 0e00  Nr....r....).r..
-00000800: 0000 7218 0000 0072 0c00 0000 720c 0000  ..r....r....r...
-00000810: 0072 0d00 0000 721a 0000 0035 0000 0073  .r....r....5...s
-00000820: 0600 0000 0002 0201 02ff 7a0c 4361 6c6c  ..........z.Call
-00000830: 2e74 6f5f 6a73 6f6e 721b 0000 0063 0100  .to_jsonr....c..
-00000840: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00000850: 0000 4300 0001 7308 0000 0064 0169 0069  ..C...s....d.i.i
-00000860: 0153 0029 024e 721f 0000 0072 0c00 0000  .S.).Nr....r....
-00000870: 7218 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
-00000880: 0d00 0000 721c 0000 003b 0000 0073 0400  ....r....;...s..
-00000890: 0000 0003 04ff 7a11 4361 6c6c 2e74 6f5f  ......z.Call.to_
-000008a0: 656e 636f 6461 626c 654e 721d 0000 0072  encodableNr....r
-000008b0: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-000008c0: 0000 0072 1f00 0000 3000 0000 730c 0000  ...r....0...s...
-000008d0: 000a 020c 010c 0202 0110 0502 0172 1f00  .............r..
-000008e0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-000008f0: 0000 0004 0000 0040 0000 0173 4a00 0000  .......@...sJ...
-00000900: 6500 5a01 6400 5a02 5500 6401 5a03 6402  e.Z.d.Z.U.d.Z.d.
-00000910: 6504 6403 3c00 6400 5a05 6402 6504 6404  e.d.<.d.Z.d.e.d.
-00000920: 3c00 6506 6405 6406 9c01 6407 6408 8404  <.e.d.d...d.d...
-00000930: 8301 5a07 6506 6409 6406 9c01 640a 640b  ..Z.e.d.d...d.d.
-00000940: 8404 8301 5a08 640c 5300 290d da03 5075  ....Z.d.S.)...Pu
-00000950: 74e9 0200 0000 7213 0000 0072 1400 0000  t.....r....r....
-00000960: 7206 0000 0072 0f00 0000 7215 0000 0063  r....r....r....c
-00000970: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000980: 0300 0000 4300 0001 730a 0000 0074 0064  ....C...s....t.d
-00000990: 0164 028d 0153 0029 034e 7221 0000 0072  .d...S.).Nr!...r
-000009a0: 1700 0000 2901 720f 0000 0072 1800 0000  ....).r....r....
-000009b0: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
-000009c0: 1a00 0000 4700 0000 7306 0000 0000 0202  ....G...s.......
-000009d0: 0102 ff7a 0b50 7574 2e74 6f5f 6a73 6f6e  ...z.Put.to_json
-000009e0: 721b 0000 0063 0100 0000 0000 0000 0000  r....c..........
-000009f0: 0000 0100 0000 0200 0000 4300 0001 7308  ..........C...s.
-00000a00: 0000 0064 0169 0069 0153 0029 024e 7221  ...d.i.i.S.).Nr!
-00000a10: 0000 0072 0c00 0000 7218 0000 0072 0c00  ...r....r....r..
-00000a20: 0000 720c 0000 0072 0d00 0000 721c 0000  ..r....r....r...
-00000a30: 004d 0000 0073 0400 0000 0003 04ff 7a10  .M...s........z.
-00000a40: 5075 742e 746f 5f65 6e63 6f64 6162 6c65  Put.to_encodable
-00000a50: 4e72 1d00 0000 720c 0000 0072 0c00 0000  Nr....r....r....
-00000a60: 720c 0000 0072 0d00 0000 7221 0000 0042  r....r....r!...B
-00000a70: 0000 0073 0c00 0000 0a02 0c01 0c02 0201  ...s............
-00000a80: 1005 0201 7221 0000 0063 0000 0000 0000  ....r!...c......
-00000a90: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
-00000aa0: 0001 734a 0000 0065 005a 0164 005a 0255  ..sJ...e.Z.d.Z.U
-00000ab0: 0064 015a 0364 0265 0464 033c 0064 005a  .d.Z.d.e.d.<.d.Z
-00000ac0: 0564 0265 0464 043c 0065 0664 0564 069c  .d.e.d.<.e.d.d..
-00000ad0: 0164 0764 0884 0483 015a 0765 0664 0964  .d.d.....Z.e.d.d
-00000ae0: 069c 0164 0a64 0b84 0483 015a 0864 0c53  ...d.d.....Z.d.S
-00000af0: 0029 0dda 0646 7574 7572 65e9 0300 0000  .)...Future.....
-00000b00: 7213 0000 0072 1400 0000 7206 0000 0072  r....r....r....r
-00000b10: 1000 0000 7215 0000 0063 0100 0000 0000  ....r....c......
-00000b20: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00000b30: 0001 730a 0000 0074 0064 0164 028d 0153  ..s....t.d.d...S
-00000b40: 0029 034e 7223 0000 0072 1700 0000 2901  .).Nr#...r....).
-00000b50: 7210 0000 0072 1800 0000 720c 0000 0072  r....r....r....r
-00000b60: 0c00 0000 720d 0000 0072 1a00 0000 5900  ....r....r....Y.
-00000b70: 0000 7306 0000 0000 0202 0102 ff7a 0e46  ..s..........z.F
-00000b80: 7574 7572 652e 746f 5f6a 736f 6e72 1b00  uture.to_jsonr..
-00000b90: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00000ba0: 0000 0002 0000 0043 0000 0173 0800 0000  .......C...s....
-00000bb0: 6401 6900 6901 5300 2902 4e72 2300 0000  d.i.i.S.).Nr#...
-00000bc0: 720c 0000 0072 1800 0000 720c 0000 0072  r....r....r....r
-00000bd0: 0c00 0000 720d 0000 0072 1c00 0000 5f00  ....r....r...._.
-00000be0: 0000 7304 0000 0000 0304 ff7a 1346 7574  ..s........z.Fut
-00000bf0: 7572 652e 746f 5f65 6e63 6f64 6162 6c65  ure.to_encodable
-00000c00: 4e72 1d00 0000 720c 0000 0072 0c00 0000  Nr....r....r....
-00000c10: 720c 0000 0072 0d00 0000 7223 0000 0054  r....r....r#...T
-00000c20: 0000 0073 0c00 0000 0a02 0c01 0c02 0201  ...s............
-00000c30: 1005 0201 7223 0000 0063 0000 0000 0000  ....r#...c......
-00000c40: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
-00000c50: 0001 734a 0000 0065 005a 0164 005a 0255  ..sJ...e.Z.d.Z.U
-00000c60: 0064 015a 0364 0265 0464 033c 0064 005a  .d.Z.d.e.d.<.d.Z
-00000c70: 0564 0265 0464 043c 0065 0664 0564 069c  .d.e.d.<.e.d.d..
-00000c80: 0164 0764 0884 0483 015a 0765 0664 0964  .d.d.....Z.e.d.d
-00000c90: 069c 0164 0a64 0b84 0483 015a 0864 0c53  ...d.d.....Z.d.S
-00000ca0: 0029 0dda 0450 6572 70e9 0400 0000 7213  .)...Perp.....r.
-00000cb0: 0000 0072 1400 0000 7206 0000 0072 1100  ...r....r....r..
-00000cc0: 0000 7215 0000 0063 0100 0000 0000 0000  ..r....c........
-00000cd0: 0000 0000 0100 0000 0300 0000 4300 0001  ............C...
-00000ce0: 730a 0000 0074 0064 0164 028d 0153 0029  s....t.d.d...S.)
-00000cf0: 034e 7225 0000 0072 1700 0000 2901 7211  .Nr%...r....).r.
-00000d00: 0000 0072 1800 0000 720c 0000 0072 0c00  ...r....r....r..
-00000d10: 0000 720d 0000 0072 1a00 0000 6b00 0000  ..r....r....k...
-00000d20: 7306 0000 0000 0202 0102 ff7a 0c50 6572  s..........z.Per
-00000d30: 702e 746f 5f6a 736f 6e72 1b00 0000 6301  p.to_jsonr....c.
-00000d40: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00000d50: 0000 0043 0000 0173 0800 0000 6401 6900  ...C...s....d.i.
-00000d60: 6901 5300 2902 4e72 2500 0000 720c 0000  i.S.).Nr%...r...
-00000d70: 0072 1800 0000 720c 0000 0072 0c00 0000  .r....r....r....
-00000d80: 720d 0000 0072 1c00 0000 7100 0000 7304  r....r....q...s.
-00000d90: 0000 0000 0304 ff7a 1150 6572 702e 746f  .......z.Perp.to
-00000da0: 5f65 6e63 6f64 6162 6c65 4e72 1d00 0000  _encodableNr....
-00000db0: 720c 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
-00000dc0: 0d00 0000 7225 0000 0066 0000 0073 0c00  ....r%...f...s..
-00000dd0: 0000 0a02 0c01 0c02 0201 1005 0201 7225  ..............r%
-00000de0: 0000 0072 1b00 0000 da08 4b69 6e64 4b69  ...r......KindKi
-00000df0: 6e64 2902 da03 6f62 6a72 1600 0000 6301  nd)...objr....c.
-00000e00: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00000e10: 0000 0043 0000 0173 6400 0000 7400 7c00  ...C...sd...t.|.
-00000e20: 7401 8302 7312 7402 6401 8301 8201 6402  t...s.t.d.....d.
-00000e30: 7c00 7600 7220 7403 8300 5300 6403 7c00  |.v.r t...S.d.|.
-00000e40: 7600 722e 7404 8300 5300 6404 7c00 7600  v.r.t...S.d.|.v.
-00000e50: 723c 7405 8300 5300 6405 7c00 7600 724a  r<t...S.d.|.v.rJ
-00000e60: 7406 8300 5300 6406 7c00 7600 7258 7407  t...S.d.|.v.rXt.
-00000e70: 8300 5300 7402 6401 8301 8201 6400 5300  ..S.t.d.....d.S.
-00000e80: 2907 4e7a 1349 6e76 616c 6964 2065 6e75  ).Nz.Invalid enu
-00000e90: 6d20 6f62 6a65 6374 7212 0000 0072 1f00  m objectr....r..
-00000ea0: 0000 7221 0000 0072 2300 0000 7225 0000  ..r!...r#...r%..
-00000eb0: 0029 08da 0a69 7369 6e73 7461 6e63 6572  .)...isinstancer
-00000ec0: 1b00 0000 da0a 5661 6c75 6545 7272 6f72  ......ValueError
-00000ed0: 7212 0000 0072 1f00 0000 7221 0000 0072  r....r....r!...r
-00000ee0: 2300 0000 7225 0000 0029 0172 2800 0000  #...r%...).r(...
-00000ef0: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00000f00: 0c66 726f 6d5f 6465 636f 6465 647c 0000  .from_decoded|..
-00000f10: 0073 1a00 0000 0001 0a01 0801 0801 0601  .s..............
-00000f20: 0801 0601 0801 0601 0801 0601 0801 0601  ................
-00000f30: 722b 0000 00da 084b 696e 644a 534f 4e63  r+.....KindJSONc
-00000f40: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000f50: 0300 0000 4300 0001 7374 0000 007c 0064  ....C...st...|.d
-00000f60: 0119 0064 026b 0272 1274 0083 0053 007c  ...d.k.r.t...S.|
-00000f70: 0064 0119 0064 036b 0272 2474 0183 0053  .d...d.k.r$t...S
-00000f80: 007c 0064 0119 0064 046b 0272 3674 0283  .|.d...d.k.r6t..
-00000f90: 0053 007c 0064 0119 0064 056b 0272 4874  .S.|.d...d.k.rHt
-00000fa0: 0383 0053 007c 0064 0119 0064 066b 0272  ...S.|.d...d.k.r
-00000fb0: 5a74 0483 0053 007c 0064 0119 007d 0174  Zt...S.|.d...}.t
-00000fc0: 0564 077c 019b 009d 0283 0182 0164 0053  .d.|.........d.S
-00000fd0: 0029 084e 7206 0000 0072 1200 0000 721f  .).Nr....r....r.
-00000fe0: 0000 0072 2100 0000 7223 0000 0072 2500  ...r!...r#...r%.
-00000ff0: 0000 7a18 556e 7265 636f 676e 697a 6564  ..z.Unrecognized
-00001000: 2065 6e75 6d20 6b69 6e64 3a20 2906 7212   enum kind: ).r.
-00001010: 0000 0072 1f00 0000 7221 0000 0072 2300  ...r....r!...r#.
-00001020: 0000 7225 0000 0072 2a00 0000 2902 7228  ..r%...r*...).r(
-00001030: 0000 0072 0600 0000 720c 0000 0072 0c00  ...r....r....r..
-00001040: 0000 720d 0000 00da 0966 726f 6d5f 6a73  ..r......from_js
-00001050: 6f6e 8c00 0000 7318 0000 0000 010c 0106  on....s.........
-00001060: 010c 0106 010c 0106 010c 0106 010c 0106  ................
-00001070: 0108 0172 2d00 0000 291b da0a 5f5f 6675  ...r-...)...__fu
-00001080: 7475 7265 5f5f 7202 0000 00da 0674 7970  ture__r......typ
-00001090: 696e 67da 0b64 6174 6163 6c61 7373 6573  ing..dataclasses
-000010a0: 7203 0000 00da 0f62 6f72 7368 5f63 6f6e  r......borsh_con
-000010b0: 7374 7275 6374 da05 626f 7273 68da 1861  struct..borsh..a
-000010c0: 6e63 686f 7270 792e 626f 7273 685f 6578  nchorpy.borsh_ex
-000010d0: 7465 6e73 696f 6e72 0400 0000 da09 5479  tensionr......Ty
-000010e0: 7065 6444 6963 7472 0500 0000 720e 0000  pedDictr....r...
-000010f0: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
-00001100: 7212 0000 0072 1f00 0000 7221 0000 0072  r....r....r!...r
-00001110: 2300 0000 7225 0000 00da 0555 6e69 6f6e  #...r%.....Union
-00001120: 7227 0000 0072 2c00 0000 722b 0000 0072  r'...r,...r+...r
-00001130: 2d00 0000 da07 4353 7472 7563 74da 066c  -.....CStruct..l
-00001140: 6179 6f75 7472 0c00 0000 720c 0000 0072  ayoutr....r....r
-00001150: 0c00 0000 720d 0000 00da 083c 6d6f 6475  ....r......<modu
-00001160: 6c65 3e01 0000 0073 3c00 0000 0c02 0801  le>....s<.......
-00001170: 0c02 0801 0c03 1204 1204 1204 1204 1204  ................
-00001180: 0201 1011 0201 1011 0201 1011 0201 1011  ................
-00001190: 0201 1011 1401 1403 1010 100f 0201 0a01  ................
-000011a0: 0a01 0a01 0a01 0afb                      ........
+00000200: 6403 5300 2904 da09 4c69 6d69 744a 534f  d.S.)...LimitJSO
+00000210: 4e7a 1774 7970 696e 672e 4c69 7465 7261  Nz.typing.Litera
+00000220: 6c5b 274c 696d 6974 275d da04 6b69 6e64  l['Limit']..kind
+00000230: 4ea9 04da 085f 5f6e 616d 655f 5fda 0a5f  N....__name__.._
+00000240: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000250: 6c6e 616d 655f 5fda 0f5f 5f61 6e6e 6f74  lname__..__annot
+00000260: 6174 696f 6e73 5f5f a900 720c 0000 0072  ations__..r....r
+00000270: 0c00 0000 fa4d 2f55 7365 7273 2f74 6672  .....M/Users/tfr
+00000280: 697a 7a61 2f44 6f63 756d 656e 7473 2f7a  izza/Documents/z
+00000290: 6574 612f 7a65 7461 2d70 792f 7a65 7461  eta/zeta-py/zeta
+000002a0: 5f70 792f 7a65 7461 5f63 6c69 656e 742f  _py/zeta_client/
+000002b0: 7479 7065 732f 6f72 6465 725f 7479 7065  types/order_type
+000002c0: 2e70 7972 0500 0000 0a00 0000 7302 0000  .pyr........s...
+000002d0: 000a 0172 0500 0000 6300 0000 0000 0000  ...r....c.......
+000002e0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+000002f0: 0173 1600 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
+00000300: 6401 6503 6402 3c00 6403 5300 2904 da0c  d.e.d.<.d.S.)...
+00000310: 506f 7374 4f6e 6c79 4a53 4f4e 7a1a 7479  PostOnlyJSONz.ty
+00000320: 7069 6e67 2e4c 6974 6572 616c 5b27 506f  ping.Literal['Po
+00000330: 7374 4f6e 6c79 275d 7206 0000 004e 7207  stOnly']r....Nr.
+00000340: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
+00000350: 0000 720d 0000 0072 0e00 0000 0e00 0000  ..r....r........
+00000360: 7302 0000 000a 0172 0e00 0000 6300 0000  s......r....c...
+00000370: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00000380: 0040 0000 0173 1600 0000 6500 5a01 6400  .@...s....e.Z.d.
+00000390: 5a02 5500 6401 6503 6402 3c00 6403 5300  Z.U.d.e.d.<.d.S.
+000003a0: 2904 da0e 4669 6c6c 4f72 4b69 6c6c 4a53  )...FillOrKillJS
+000003b0: 4f4e 7a1c 7479 7069 6e67 2e4c 6974 6572  ONz.typing.Liter
+000003c0: 616c 5b27 4669 6c6c 4f72 4b69 6c6c 275d  al['FillOrKill']
+000003d0: 7206 0000 004e 7207 0000 0072 0c00 0000  r....Nr....r....
+000003e0: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+000003f0: 0f00 0000 1200 0000 7302 0000 000a 0172  ........s......r
+00000400: 0f00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000410: 0000 0000 0003 0000 0040 0000 0173 1600  .........@...s..
+00000420: 0000 6500 5a01 6400 5a02 5500 6401 6503  ..e.Z.d.Z.U.d.e.
+00000430: 6402 3c00 6403 5300 2904 da15 496d 6d65  d.<.d.S.)...Imme
+00000440: 6469 6174 654f 7243 616e 6365 6c4a 534f  diateOrCancelJSO
+00000450: 4e7a 2374 7970 696e 672e 4c69 7465 7261  Nz#typing.Litera
+00000460: 6c5b 2749 6d6d 6564 6961 7465 4f72 4361  l['ImmediateOrCa
+00000470: 6e63 656c 275d 7206 0000 004e 7207 0000  ncel']r....Nr...
+00000480: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
+00000490: 720d 0000 0072 1000 0000 1600 0000 7302  r....r........s.
+000004a0: 0000 000a 0172 1000 0000 6300 0000 0000  .....r....c.....
+000004b0: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
+000004c0: 0000 0173 1600 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+000004d0: 5500 6401 6503 6402 3c00 6403 5300 2904  U.d.e.d.<.d.S.).
+000004e0: da11 506f 7374 4f6e 6c79 536c 6964 654a  ..PostOnlySlideJ
+000004f0: 534f 4e7a 1f74 7970 696e 672e 4c69 7465  SONz.typing.Lite
+00000500: 7261 6c5b 2750 6f73 744f 6e6c 7953 6c69  ral['PostOnlySli
+00000510: 6465 275d 7206 0000 004e 7207 0000 0072  de']r....Nr....r
+00000520: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
+00000530: 0000 0072 1100 0000 1a00 0000 7302 0000  ...r........s...
+00000540: 000a 0172 1100 0000 6300 0000 0000 0000  ...r....c.......
+00000550: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
+00000560: 0173 4a00 0000 6500 5a01 6400 5a02 5500  .sJ...e.Z.d.Z.U.
+00000570: 6401 5a03 6402 6504 6403 3c00 6400 5a05  d.Z.d.e.d.<.d.Z.
+00000580: 6402 6504 6404 3c00 6506 6405 6406 9c01  d.e.d.<.e.d.d...
+00000590: 6407 6408 8404 8301 5a07 6506 6409 6406  d.d.....Z.e.d.d.
+000005a0: 9c01 640a 640b 8404 8301 5a08 640c 5300  ..d.d.....Z.d.S.
+000005b0: 290d da05 4c69 6d69 7472 0100 0000 fa0f  )...Limitr......
+000005c0: 7479 7069 6e67 2e43 6c61 7373 5661 72da  typing.ClassVar.
+000005d0: 0d64 6973 6372 696d 696e 6174 6f72 7206  .discriminatorr.
+000005e0: 0000 0072 0500 0000 a901 da06 7265 7475  ...r........retu
+000005f0: 726e 6301 0000 0000 0000 0000 0000 0001  rnc.............
+00000600: 0000 0003 0000 0043 0000 0173 0a00 0000  .......C...s....
+00000610: 7400 6401 6402 8d01 5300 2903 4e72 1200  t.d.d...S.).Nr..
+00000620: 0000 a901 7206 0000 0029 0172 0500 0000  ....r....).r....
+00000630: a901 da03 636c 7372 0c00 0000 720c 0000  ....clsr....r...
+00000640: 0072 0d00 0000 da07 746f 5f6a 736f 6e23  .r......to_json#
+00000650: 0000 0073 0600 0000 0002 0201 02ff 7a0d  ...s..........z.
+00000660: 4c69 6d69 742e 746f 5f6a 736f 6eda 0464  Limit.to_json..d
+00000670: 6963 7463 0100 0000 0000 0000 0000 0000  ictc............
+00000680: 0100 0000 0200 0000 4300 0001 7308 0000  ........C...s...
+00000690: 0064 0169 0069 0153 0029 024e 7212 0000  .d.i.i.S.).Nr...
+000006a0: 0072 0c00 0000 7218 0000 0072 0c00 0000  .r....r....r....
+000006b0: 720c 0000 0072 0d00 0000 da0c 746f 5f65  r....r......to_e
+000006c0: 6e63 6f64 6162 6c65 2900 0000 7304 0000  ncodable)...s...
+000006d0: 0000 0304 ff7a 124c 696d 6974 2e74 6f5f  .....z.Limit.to_
+000006e0: 656e 636f 6461 626c 654e a909 7208 0000  encodableN..r...
+000006f0: 0072 0900 0000 720a 0000 0072 1400 0000  .r....r....r....
+00000700: 720b 0000 0072 0600 0000 da0b 636c 6173  r....r......clas
+00000710: 736d 6574 686f 6472 1a00 0000 721c 0000  smethodr....r...
+00000720: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
+00000730: 720d 0000 0072 1200 0000 1e00 0000 730c  r....r........s.
+00000740: 0000 000a 020c 010c 0202 0110 0502 0172  ...............r
+00000750: 1200 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000760: 0000 0000 0004 0000 0040 0000 0173 4a00  .........@...sJ.
+00000770: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
+00000780: 6402 6504 6403 3c00 6400 5a05 6402 6504  d.e.d.<.d.Z.d.e.
+00000790: 6404 3c00 6506 6405 6406 9c01 6407 6408  d.<.e.d.d...d.d.
+000007a0: 8404 8301 5a07 6506 6409 6406 9c01 640a  ....Z.e.d.d...d.
+000007b0: 640b 8404 8301 5a08 640c 5300 290d da08  d.....Z.d.S.)...
+000007c0: 506f 7374 4f6e 6c79 e901 0000 0072 1300  PostOnly.....r..
+000007d0: 0000 7214 0000 0072 0600 0000 720e 0000  ..r....r....r...
+000007e0: 0072 1500 0000 6301 0000 0000 0000 0000  .r....c.........
+000007f0: 0000 0001 0000 0003 0000 0043 0000 0173  ...........C...s
+00000800: 0a00 0000 7400 6401 6402 8d01 5300 2903  ....t.d.d...S.).
+00000810: 4e72 1f00 0000 7217 0000 0029 0172 0e00  Nr....r....).r..
+00000820: 0000 7218 0000 0072 0c00 0000 720c 0000  ..r....r....r...
+00000830: 0072 0d00 0000 721a 0000 0035 0000 0073  .r....r....5...s
+00000840: 0600 0000 0002 0201 02ff 7a10 506f 7374  ..........z.Post
+00000850: 4f6e 6c79 2e74 6f5f 6a73 6f6e 721b 0000  Only.to_jsonr...
+00000860: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00000870: 0000 0200 0000 4300 0001 7308 0000 0064  ......C...s....d
+00000880: 0169 0069 0153 0029 024e 721f 0000 0072  .i.i.S.).Nr....r
+00000890: 0c00 0000 7218 0000 0072 0c00 0000 720c  ....r....r....r.
+000008a0: 0000 0072 0d00 0000 721c 0000 003b 0000  ...r....r....;..
+000008b0: 0073 0400 0000 0003 04ff 7a15 506f 7374  .s........z.Post
+000008c0: 4f6e 6c79 2e74 6f5f 656e 636f 6461 626c  Only.to_encodabl
+000008d0: 654e 721d 0000 0072 0c00 0000 720c 0000  eNr....r....r...
+000008e0: 0072 0c00 0000 720d 0000 0072 1f00 0000  .r....r....r....
+000008f0: 3000 0000 730c 0000 000a 020c 010c 0202  0...s...........
+00000900: 0110 0502 0172 1f00 0000 6300 0000 0000  .....r....c.....
+00000910: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
+00000920: 0000 0173 4a00 0000 6500 5a01 6400 5a02  ...sJ...e.Z.d.Z.
+00000930: 5500 6401 5a03 6402 6504 6403 3c00 6400  U.d.Z.d.e.d.<.d.
+00000940: 5a05 6402 6504 6404 3c00 6506 6405 6406  Z.d.e.d.<.e.d.d.
+00000950: 9c01 6407 6408 8404 8301 5a07 6506 6409  ..d.d.....Z.e.d.
+00000960: 6406 9c01 640a 640b 8404 8301 5a08 640c  d...d.d.....Z.d.
+00000970: 5300 290d da0a 4669 6c6c 4f72 4b69 6c6c  S.)...FillOrKill
+00000980: e902 0000 0072 1300 0000 7214 0000 0072  .....r....r....r
+00000990: 0600 0000 720f 0000 0072 1500 0000 6301  ....r....r....c.
+000009a0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+000009b0: 0000 0043 0000 0173 0a00 0000 7400 6401  ...C...s....t.d.
+000009c0: 6402 8d01 5300 2903 4e72 2100 0000 7217  d...S.).Nr!...r.
+000009d0: 0000 0029 0172 0f00 0000 7218 0000 0072  ...).r....r....r
+000009e0: 0c00 0000 720c 0000 0072 0d00 0000 721a  ....r....r....r.
+000009f0: 0000 0047 0000 0073 0600 0000 0002 0201  ...G...s........
+00000a00: 02ff 7a12 4669 6c6c 4f72 4b69 6c6c 2e74  ..z.FillOrKill.t
+00000a10: 6f5f 6a73 6f6e 721b 0000 0063 0100 0000  o_jsonr....c....
+00000a20: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00000a30: 4300 0001 7308 0000 0064 0169 0069 0153  C...s....d.i.i.S
+00000a40: 0029 024e 7221 0000 0072 0c00 0000 7218  .).Nr!...r....r.
+00000a50: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+00000a60: 0000 721c 0000 004d 0000 0073 0400 0000  ..r....M...s....
+00000a70: 0003 04ff 7a17 4669 6c6c 4f72 4b69 6c6c  ....z.FillOrKill
+00000a80: 2e74 6f5f 656e 636f 6461 626c 654e 721d  .to_encodableNr.
+00000a90: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
+00000aa0: 0000 720d 0000 0072 2100 0000 4200 0000  ..r....r!...B...
+00000ab0: 730c 0000 000a 020c 010c 0202 0110 0502  s...............
+00000ac0: 0172 2100 0000 6300 0000 0000 0000 0000  .r!...c.........
+00000ad0: 0000 0000 0000 0004 0000 0040 0000 0173  ...........@...s
+00000ae0: 4a00 0000 6500 5a01 6400 5a02 5500 6401  J...e.Z.d.Z.U.d.
+00000af0: 5a03 6402 6504 6403 3c00 6400 5a05 6402  Z.d.e.d.<.d.Z.d.
+00000b00: 6504 6404 3c00 6506 6405 6406 9c01 6407  e.d.<.e.d.d...d.
+00000b10: 6408 8404 8301 5a07 6506 6409 6406 9c01  d.....Z.e.d.d...
+00000b20: 640a 640b 8404 8301 5a08 640c 5300 290d  d.d.....Z.d.S.).
+00000b30: da11 496d 6d65 6469 6174 654f 7243 616e  ..ImmediateOrCan
+00000b40: 6365 6ce9 0300 0000 7213 0000 0072 1400  cel.....r....r..
+00000b50: 0000 7206 0000 0072 1000 0000 7215 0000  ..r....r....r...
+00000b60: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00000b70: 0000 0300 0000 4300 0001 730a 0000 0074  ......C...s....t
+00000b80: 0064 0164 028d 0153 0029 034e 7223 0000  .d.d...S.).Nr#..
+00000b90: 0072 1700 0000 2901 7210 0000 0072 1800  .r....).r....r..
+00000ba0: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+00000bb0: 0072 1a00 0000 5900 0000 7306 0000 0000  .r....Y...s.....
+00000bc0: 0202 0102 ff7a 1949 6d6d 6564 6961 7465  .....z.Immediate
+00000bd0: 4f72 4361 6e63 656c 2e74 6f5f 6a73 6f6e  OrCancel.to_json
+00000be0: 721b 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00000bf0: 0000 0100 0000 0200 0000 4300 0001 7308  ..........C...s.
+00000c00: 0000 0064 0169 0069 0153 0029 024e 7223  ...d.i.i.S.).Nr#
+00000c10: 0000 0072 0c00 0000 7218 0000 0072 0c00  ...r....r....r..
+00000c20: 0000 720c 0000 0072 0d00 0000 721c 0000  ..r....r....r...
+00000c30: 005f 0000 0073 0400 0000 0003 04ff 7a1e  ._...s........z.
+00000c40: 496d 6d65 6469 6174 654f 7243 616e 6365  ImmediateOrCance
+00000c50: 6c2e 746f 5f65 6e63 6f64 6162 6c65 4e72  l.to_encodableNr
+00000c60: 1d00 0000 720c 0000 0072 0c00 0000 720c  ....r....r....r.
+00000c70: 0000 0072 0d00 0000 7223 0000 0054 0000  ...r....r#...T..
+00000c80: 0073 0c00 0000 0a02 0c01 0c02 0201 1005  .s..............
+00000c90: 0201 7223 0000 0063 0000 0000 0000 0000  ..r#...c........
+00000ca0: 0000 0000 0000 0000 0400 0000 4000 0001  ............@...
+00000cb0: 734a 0000 0065 005a 0164 005a 0255 0064  sJ...e.Z.d.Z.U.d
+00000cc0: 015a 0364 0265 0464 033c 0064 005a 0564  .Z.d.e.d.<.d.Z.d
+00000cd0: 0265 0464 043c 0065 0664 0564 069c 0164  .e.d.<.e.d.d...d
+00000ce0: 0764 0884 0483 015a 0765 0664 0964 069c  .d.....Z.e.d.d..
+00000cf0: 0164 0a64 0b84 0483 015a 0864 0c53 0029  .d.d.....Z.d.S.)
+00000d00: 0dda 0d50 6f73 744f 6e6c 7953 6c69 6465  ...PostOnlySlide
+00000d10: e904 0000 0072 1300 0000 7214 0000 0072  .....r....r....r
+00000d20: 0600 0000 7211 0000 0072 1500 0000 6301  ....r....r....c.
+00000d30: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00000d40: 0000 0043 0000 0173 0a00 0000 7400 6401  ...C...s....t.d.
+00000d50: 6402 8d01 5300 2903 4e72 2500 0000 7217  d...S.).Nr%...r.
+00000d60: 0000 0029 0172 1100 0000 7218 0000 0072  ...).r....r....r
+00000d70: 0c00 0000 720c 0000 0072 0d00 0000 721a  ....r....r....r.
+00000d80: 0000 006b 0000 0073 0600 0000 0002 0201  ...k...s........
+00000d90: 02ff 7a15 506f 7374 4f6e 6c79 536c 6964  ..z.PostOnlySlid
+00000da0: 652e 746f 5f6a 736f 6e72 1b00 0000 6301  e.to_jsonr....c.
+00000db0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00000dc0: 0000 0043 0000 0173 0800 0000 6401 6900  ...C...s....d.i.
+00000dd0: 6901 5300 2902 4e72 2500 0000 720c 0000  i.S.).Nr%...r...
+00000de0: 0072 1800 0000 720c 0000 0072 0c00 0000  .r....r....r....
+00000df0: 720d 0000 0072 1c00 0000 7100 0000 7304  r....r....q...s.
+00000e00: 0000 0000 0304 ff7a 1a50 6f73 744f 6e6c  .......z.PostOnl
+00000e10: 7953 6c69 6465 2e74 6f5f 656e 636f 6461  ySlide.to_encoda
+00000e20: 626c 654e 721d 0000 0072 0c00 0000 720c  bleNr....r....r.
+00000e30: 0000 0072 0c00 0000 720d 0000 0072 2500  ...r....r....r%.
+00000e40: 0000 6600 0000 730c 0000 000a 020c 010c  ..f...s.........
+00000e50: 0202 0110 0502 0172 2500 0000 721b 0000  .......r%...r...
+00000e60: 00da 0d4f 7264 6572 5479 7065 4b69 6e64  ...OrderTypeKind
+00000e70: 2902 da03 6f62 6a72 1600 0000 6301 0000  )...objr....c...
+00000e80: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00000e90: 0043 0000 0173 6400 0000 7400 7c00 7401  .C...sd...t.|.t.
+00000ea0: 8302 7312 7402 6401 8301 8201 6402 7c00  ..s.t.d.....d.|.
+00000eb0: 7600 7220 7403 8300 5300 6403 7c00 7600  v.r t...S.d.|.v.
+00000ec0: 722e 7404 8300 5300 6404 7c00 7600 723c  r.t...S.d.|.v.r<
+00000ed0: 7405 8300 5300 6405 7c00 7600 724a 7406  t...S.d.|.v.rJt.
+00000ee0: 8300 5300 6406 7c00 7600 7258 7407 8300  ..S.d.|.v.rXt...
+00000ef0: 5300 7402 6401 8301 8201 6400 5300 2907  S.t.d.....d.S.).
+00000f00: 4e7a 1349 6e76 616c 6964 2065 6e75 6d20  Nz.Invalid enum 
+00000f10: 6f62 6a65 6374 7212 0000 0072 1f00 0000  objectr....r....
+00000f20: 7221 0000 0072 2300 0000 7225 0000 0029  r!...r#...r%...)
+00000f30: 08da 0a69 7369 6e73 7461 6e63 6572 1b00  ...isinstancer..
+00000f40: 0000 da0a 5661 6c75 6545 7272 6f72 7212  ....ValueErrorr.
+00000f50: 0000 0072 1f00 0000 7221 0000 0072 2300  ...r....r!...r#.
+00000f60: 0000 7225 0000 0029 0172 2800 0000 720c  ..r%...).r(...r.
+00000f70: 0000 0072 0c00 0000 720d 0000 00da 0c66  ...r....r......f
+00000f80: 726f 6d5f 6465 636f 6465 647c 0000 0073  rom_decoded|...s
+00000f90: 1a00 0000 0001 0a01 0801 0801 0601 0801  ................
+00000fa0: 0601 0801 0601 0801 0601 0801 0601 722b  ..............r+
+00000fb0: 0000 00da 0d4f 7264 6572 5479 7065 4a53  .....OrderTypeJS
+00000fc0: 4f4e 6301 0000 0000 0000 0000 0000 0002  ONc.............
+00000fd0: 0000 0003 0000 0043 0000 0173 7400 0000  .......C...st...
+00000fe0: 7c00 6401 1900 6402 6b02 7212 7400 8300  |.d...d.k.r.t...
+00000ff0: 5300 7c00 6401 1900 6403 6b02 7224 7401  S.|.d...d.k.r$t.
+00001000: 8300 5300 7c00 6401 1900 6404 6b02 7236  ..S.|.d...d.k.r6
+00001010: 7402 8300 5300 7c00 6401 1900 6405 6b02  t...S.|.d...d.k.
+00001020: 7248 7403 8300 5300 7c00 6401 1900 6406  rHt...S.|.d...d.
+00001030: 6b02 725a 7404 8300 5300 7c00 6401 1900  k.rZt...S.|.d...
+00001040: 7d01 7405 6407 7c01 9b00 9d02 8301 8201  }.t.d.|.........
+00001050: 6400 5300 2908 4e72 0600 0000 7212 0000  d.S.).Nr....r...
+00001060: 0072 1f00 0000 7221 0000 0072 2300 0000  .r....r!...r#...
+00001070: 7225 0000 007a 1855 6e72 6563 6f67 6e69  r%...z.Unrecogni
+00001080: 7a65 6420 656e 756d 206b 696e 643a 2029  zed enum kind: )
+00001090: 0672 1200 0000 721f 0000 0072 2100 0000  .r....r....r!...
+000010a0: 7223 0000 0072 2500 0000 722a 0000 0029  r#...r%...r*...)
+000010b0: 0272 2800 0000 7206 0000 0072 0c00 0000  .r(...r....r....
+000010c0: 720c 0000 0072 0d00 0000 da09 6672 6f6d  r....r......from
+000010d0: 5f6a 736f 6e8c 0000 0073 1800 0000 0001  _json....s......
+000010e0: 0c01 0601 0c01 0601 0c01 0601 0c01 0601  ................
+000010f0: 0c01 0601 0801 722d 0000 0029 1bda 0a5f  ......r-...)..._
+00001100: 5f66 7574 7572 655f 5f72 0200 0000 da06  _future__r......
+00001110: 7479 7069 6e67 da0b 6461 7461 636c 6173  typing..dataclas
+00001120: 7365 7372 0300 0000 da0f 626f 7273 685f  sesr......borsh_
+00001130: 636f 6e73 7472 7563 74da 0562 6f72 7368  construct..borsh
+00001140: da18 616e 6368 6f72 7079 2e62 6f72 7368  ..anchorpy.borsh
+00001150: 5f65 7874 656e 7369 6f6e 7204 0000 00da  _extensionr.....
+00001160: 0954 7970 6564 4469 6374 7205 0000 0072  .TypedDictr....r
+00001170: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
+00001180: 0000 0072 1200 0000 721f 0000 0072 2100  ...r....r....r!.
+00001190: 0000 7223 0000 0072 2500 0000 da05 556e  ..r#...r%.....Un
+000011a0: 696f 6e72 2700 0000 722c 0000 0072 2b00  ionr'...r,...r+.
+000011b0: 0000 722d 0000 00da 0743 5374 7275 6374  ..r-.....CStruct
+000011c0: da06 6c61 796f 7574 720c 0000 0072 0c00  ..layoutr....r..
+000011d0: 0000 720c 0000 0072 0d00 0000 da08 3c6d  ..r....r......<m
+000011e0: 6f64 756c 653e 0100 0000 733c 0000 000c  odule>....s<....
+000011f0: 0208 010c 0208 010c 0312 0412 0412 0412  ................
+00001200: 0412 0402 0110 1102 0110 1102 0110 1102  ................
+00001210: 0110 1102 0110 1114 0114 0310 1010 0f02  ................
+00001220: 010a 010a 010a 010a 010a fb              ...........
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/margin_account_type.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/margin_account_type.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/margin_account_type.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/margin_account_type.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/margin_parameters.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/margin_parameters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/margin_parameters.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/margin_parameters.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/margin_requirement.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/margin_requirement.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/margin_requirement.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/margin_requirement.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/movement_type.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/movement_type.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/movement_type.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/movement_type.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/order_complete_type.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/order_complete_type.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/order_complete_type.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/order_complete_type.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/order_state.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/order_state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/order_state.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/order_state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/order_type.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/order_type.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/order_type.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/treasury_movement_type.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Aug 21 13:18:23 2023 UTC, .py size: 3690 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 1f64 e364 6a0e 0000  a........d.dj...
+00000000: 610d 0d0a 0000 0000 1f64 e364 7112 0000  a........d.dq...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0173 6c01 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6402 6c05 5a06 6400 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6502 6a09  ..G.d.d...d.e.j.
 00000070: 8303 5a0a 4700 6407 6408 8400 6408 6502  ..Z.G.d.d...d.e.
@@ -26,266 +26,289 @@
 00000190: 1b00 8305 5a1a 6402 5300 2921 e900 0000  ....Z.d.S.)!....
 000001a0: 0029 01da 0b61 6e6e 6f74 6174 696f 6e73  .)...annotations
 000001b0: 4e29 01da 0964 6174 6163 6c61 7373 2901  N)...dataclass).
 000001c0: da0e 456e 756d 466f 7243 6f64 6567 656e  ..EnumForCodegen
 000001d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 000001e0: 0003 0000 0040 0000 0173 1600 0000 6500  .....@...s....e.
 000001f0: 5a01 6400 5a02 5500 6401 6503 6402 3c00  Z.d.Z.U.d.e.d.<.
-00000200: 6403 5300 2904 da09 4c69 6d69 744a 534f  d.S.)...LimitJSO
-00000210: 4e7a 1774 7970 696e 672e 4c69 7465 7261  Nz.typing.Litera
-00000220: 6c5b 274c 696d 6974 275d da04 6b69 6e64  l['Limit']..kind
-00000230: 4ea9 04da 085f 5f6e 616d 655f 5fda 0a5f  N....__name__.._
-00000240: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000250: 6c6e 616d 655f 5fda 0f5f 5f61 6e6e 6f74  lname__..__annot
-00000260: 6174 696f 6e73 5f5f a900 720c 0000 0072  ations__..r....r
-00000270: 0c00 0000 fa4d 2f55 7365 7273 2f74 6672  .....M/Users/tfr
-00000280: 697a 7a61 2f44 6f63 756d 656e 7473 2f7a  izza/Documents/z
-00000290: 6574 612f 7a65 7461 2d70 792f 7a65 7461  eta/zeta-py/zeta
-000002a0: 5f70 792f 7a65 7461 5f63 6c69 656e 742f  _py/zeta_client/
-000002b0: 7479 7065 732f 6f72 6465 725f 7479 7065  types/order_type
-000002c0: 2e70 7972 0500 0000 0a00 0000 7302 0000  .pyr........s...
-000002d0: 000a 0172 0500 0000 6300 0000 0000 0000  ...r....c.......
-000002e0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-000002f0: 0173 1600 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
-00000300: 6401 6503 6402 3c00 6403 5300 2904 da0c  d.e.d.<.d.S.)...
-00000310: 506f 7374 4f6e 6c79 4a53 4f4e 7a1a 7479  PostOnlyJSONz.ty
-00000320: 7069 6e67 2e4c 6974 6572 616c 5b27 506f  ping.Literal['Po
-00000330: 7374 4f6e 6c79 275d 7206 0000 004e 7207  stOnly']r....Nr.
-00000340: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
-00000350: 0000 720d 0000 0072 0e00 0000 0e00 0000  ..r....r........
-00000360: 7302 0000 000a 0172 0e00 0000 6300 0000  s......r....c...
-00000370: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00000380: 0040 0000 0173 1600 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000390: 5a02 5500 6401 6503 6402 3c00 6403 5300  Z.U.d.e.d.<.d.S.
-000003a0: 2904 da0e 4669 6c6c 4f72 4b69 6c6c 4a53  )...FillOrKillJS
-000003b0: 4f4e 7a1c 7479 7069 6e67 2e4c 6974 6572  ONz.typing.Liter
-000003c0: 616c 5b27 4669 6c6c 4f72 4b69 6c6c 275d  al['FillOrKill']
-000003d0: 7206 0000 004e 7207 0000 0072 0c00 0000  r....Nr....r....
-000003e0: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
-000003f0: 0f00 0000 1200 0000 7302 0000 000a 0172  ........s......r
-00000400: 0f00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000410: 0000 0000 0003 0000 0040 0000 0173 1600  .........@...s..
-00000420: 0000 6500 5a01 6400 5a02 5500 6401 6503  ..e.Z.d.Z.U.d.e.
-00000430: 6402 3c00 6403 5300 2904 da15 496d 6d65  d.<.d.S.)...Imme
-00000440: 6469 6174 654f 7243 616e 6365 6c4a 534f  diateOrCancelJSO
-00000450: 4e7a 2374 7970 696e 672e 4c69 7465 7261  Nz#typing.Litera
-00000460: 6c5b 2749 6d6d 6564 6961 7465 4f72 4361  l['ImmediateOrCa
-00000470: 6e63 656c 275d 7206 0000 004e 7207 0000  ncel']r....Nr...
-00000480: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
-00000490: 720d 0000 0072 1000 0000 1600 0000 7302  r....r........s.
-000004a0: 0000 000a 0172 1000 0000 6300 0000 0000  .....r....c.....
-000004b0: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-000004c0: 0000 0173 1600 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-000004d0: 5500 6401 6503 6402 3c00 6403 5300 2904  U.d.e.d.<.d.S.).
-000004e0: da11 506f 7374 4f6e 6c79 536c 6964 654a  ..PostOnlySlideJ
-000004f0: 534f 4e7a 1f74 7970 696e 672e 4c69 7465  SONz.typing.Lite
-00000500: 7261 6c5b 2750 6f73 744f 6e6c 7953 6c69  ral['PostOnlySli
-00000510: 6465 275d 7206 0000 004e 7207 0000 0072  de']r....Nr....r
-00000520: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-00000530: 0000 0072 1100 0000 1a00 0000 7302 0000  ...r........s...
-00000540: 000a 0172 1100 0000 6300 0000 0000 0000  ...r....c.......
-00000550: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000560: 0173 4a00 0000 6500 5a01 6400 5a02 5500  .sJ...e.Z.d.Z.U.
-00000570: 6401 5a03 6402 6504 6403 3c00 6400 5a05  d.Z.d.e.d.<.d.Z.
-00000580: 6402 6504 6404 3c00 6506 6405 6406 9c01  d.e.d.<.e.d.d...
-00000590: 6407 6408 8404 8301 5a07 6506 6409 6406  d.d.....Z.e.d.d.
-000005a0: 9c01 640a 640b 8404 8301 5a08 640c 5300  ..d.d.....Z.d.S.
-000005b0: 290d da05 4c69 6d69 7472 0100 0000 fa0f  )...Limitr......
-000005c0: 7479 7069 6e67 2e43 6c61 7373 5661 72da  typing.ClassVar.
-000005d0: 0d64 6973 6372 696d 696e 6174 6f72 7206  .discriminatorr.
-000005e0: 0000 0072 0500 0000 a901 da06 7265 7475  ...r........retu
-000005f0: 726e 6301 0000 0000 0000 0000 0000 0001  rnc.............
-00000600: 0000 0003 0000 0043 0000 0173 0a00 0000  .......C...s....
-00000610: 7400 6401 6402 8d01 5300 2903 4e72 1200  t.d.d...S.).Nr..
-00000620: 0000 a901 7206 0000 0029 0172 0500 0000  ....r....).r....
-00000630: a901 da03 636c 7372 0c00 0000 720c 0000  ....clsr....r...
-00000640: 0072 0d00 0000 da07 746f 5f6a 736f 6e23  .r......to_json#
-00000650: 0000 0073 0600 0000 0002 0201 02ff 7a0d  ...s..........z.
-00000660: 4c69 6d69 742e 746f 5f6a 736f 6eda 0464  Limit.to_json..d
-00000670: 6963 7463 0100 0000 0000 0000 0000 0000  ictc............
-00000680: 0100 0000 0200 0000 4300 0001 7308 0000  ........C...s...
-00000690: 0064 0169 0069 0153 0029 024e 7212 0000  .d.i.i.S.).Nr...
-000006a0: 0072 0c00 0000 7218 0000 0072 0c00 0000  .r....r....r....
-000006b0: 720c 0000 0072 0d00 0000 da0c 746f 5f65  r....r......to_e
-000006c0: 6e63 6f64 6162 6c65 2900 0000 7304 0000  ncodable)...s...
-000006d0: 0000 0304 ff7a 124c 696d 6974 2e74 6f5f  .....z.Limit.to_
-000006e0: 656e 636f 6461 626c 654e a909 7208 0000  encodableN..r...
-000006f0: 0072 0900 0000 720a 0000 0072 1400 0000  .r....r....r....
-00000700: 720b 0000 0072 0600 0000 da0b 636c 6173  r....r......clas
-00000710: 736d 6574 686f 6472 1a00 0000 721c 0000  smethodr....r...
-00000720: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
-00000730: 720d 0000 0072 1200 0000 1e00 0000 730c  r....r........s.
-00000740: 0000 000a 020c 010c 0202 0110 0502 0172  ...............r
-00000750: 1200 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000760: 0000 0000 0004 0000 0040 0000 0173 4a00  .........@...sJ.
-00000770: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
-00000780: 6402 6504 6403 3c00 6400 5a05 6402 6504  d.e.d.<.d.Z.d.e.
-00000790: 6404 3c00 6506 6405 6406 9c01 6407 6408  d.<.e.d.d...d.d.
-000007a0: 8404 8301 5a07 6506 6409 6406 9c01 640a  ....Z.e.d.d...d.
-000007b0: 640b 8404 8301 5a08 640c 5300 290d da08  d.....Z.d.S.)...
-000007c0: 506f 7374 4f6e 6c79 e901 0000 0072 1300  PostOnly.....r..
-000007d0: 0000 7214 0000 0072 0600 0000 720e 0000  ..r....r....r...
-000007e0: 0072 1500 0000 6301 0000 0000 0000 0000  .r....c.........
-000007f0: 0000 0001 0000 0003 0000 0043 0000 0173  ...........C...s
-00000800: 0a00 0000 7400 6401 6402 8d01 5300 2903  ....t.d.d...S.).
-00000810: 4e72 1f00 0000 7217 0000 0029 0172 0e00  Nr....r....).r..
-00000820: 0000 7218 0000 0072 0c00 0000 720c 0000  ..r....r....r...
-00000830: 0072 0d00 0000 721a 0000 0035 0000 0073  .r....r....5...s
-00000840: 0600 0000 0002 0201 02ff 7a10 506f 7374  ..........z.Post
-00000850: 4f6e 6c79 2e74 6f5f 6a73 6f6e 721b 0000  Only.to_jsonr...
-00000860: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00000870: 0000 0200 0000 4300 0001 7308 0000 0064  ......C...s....d
-00000880: 0169 0069 0153 0029 024e 721f 0000 0072  .i.i.S.).Nr....r
-00000890: 0c00 0000 7218 0000 0072 0c00 0000 720c  ....r....r....r.
-000008a0: 0000 0072 0d00 0000 721c 0000 003b 0000  ...r....r....;..
-000008b0: 0073 0400 0000 0003 04ff 7a15 506f 7374  .s........z.Post
-000008c0: 4f6e 6c79 2e74 6f5f 656e 636f 6461 626c  Only.to_encodabl
-000008d0: 654e 721d 0000 0072 0c00 0000 720c 0000  eNr....r....r...
-000008e0: 0072 0c00 0000 720d 0000 0072 1f00 0000  .r....r....r....
-000008f0: 3000 0000 730c 0000 000a 020c 010c 0202  0...s...........
-00000900: 0110 0502 0172 1f00 0000 6300 0000 0000  .....r....c.....
-00000910: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
-00000920: 0000 0173 4a00 0000 6500 5a01 6400 5a02  ...sJ...e.Z.d.Z.
-00000930: 5500 6401 5a03 6402 6504 6403 3c00 6400  U.d.Z.d.e.d.<.d.
-00000940: 5a05 6402 6504 6404 3c00 6506 6405 6406  Z.d.e.d.<.e.d.d.
-00000950: 9c01 6407 6408 8404 8301 5a07 6506 6409  ..d.d.....Z.e.d.
-00000960: 6406 9c01 640a 640b 8404 8301 5a08 640c  d...d.d.....Z.d.
-00000970: 5300 290d da0a 4669 6c6c 4f72 4b69 6c6c  S.)...FillOrKill
-00000980: e902 0000 0072 1300 0000 7214 0000 0072  .....r....r....r
-00000990: 0600 0000 720f 0000 0072 1500 0000 6301  ....r....r....c.
-000009a0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-000009b0: 0000 0043 0000 0173 0a00 0000 7400 6401  ...C...s....t.d.
-000009c0: 6402 8d01 5300 2903 4e72 2100 0000 7217  d...S.).Nr!...r.
-000009d0: 0000 0029 0172 0f00 0000 7218 0000 0072  ...).r....r....r
-000009e0: 0c00 0000 720c 0000 0072 0d00 0000 721a  ....r....r....r.
-000009f0: 0000 0047 0000 0073 0600 0000 0002 0201  ...G...s........
-00000a00: 02ff 7a12 4669 6c6c 4f72 4b69 6c6c 2e74  ..z.FillOrKill.t
-00000a10: 6f5f 6a73 6f6e 721b 0000 0063 0100 0000  o_jsonr....c....
-00000a20: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00000a30: 4300 0001 7308 0000 0064 0169 0069 0153  C...s....d.i.i.S
-00000a40: 0029 024e 7221 0000 0072 0c00 0000 7218  .).Nr!...r....r.
-00000a50: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
-00000a60: 0000 721c 0000 004d 0000 0073 0400 0000  ..r....M...s....
-00000a70: 0003 04ff 7a17 4669 6c6c 4f72 4b69 6c6c  ....z.FillOrKill
-00000a80: 2e74 6f5f 656e 636f 6461 626c 654e 721d  .to_encodableNr.
-00000a90: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
-00000aa0: 0000 720d 0000 0072 2100 0000 4200 0000  ..r....r!...B...
-00000ab0: 730c 0000 000a 020c 010c 0202 0110 0502  s...............
-00000ac0: 0172 2100 0000 6300 0000 0000 0000 0000  .r!...c.........
-00000ad0: 0000 0000 0000 0004 0000 0040 0000 0173  ...........@...s
-00000ae0: 4a00 0000 6500 5a01 6400 5a02 5500 6401  J...e.Z.d.Z.U.d.
-00000af0: 5a03 6402 6504 6403 3c00 6400 5a05 6402  Z.d.e.d.<.d.Z.d.
-00000b00: 6504 6404 3c00 6506 6405 6406 9c01 6407  e.d.<.e.d.d...d.
-00000b10: 6408 8404 8301 5a07 6506 6409 6406 9c01  d.....Z.e.d.d...
-00000b20: 640a 640b 8404 8301 5a08 640c 5300 290d  d.d.....Z.d.S.).
-00000b30: da11 496d 6d65 6469 6174 654f 7243 616e  ..ImmediateOrCan
-00000b40: 6365 6ce9 0300 0000 7213 0000 0072 1400  cel.....r....r..
-00000b50: 0000 7206 0000 0072 1000 0000 7215 0000  ..r....r....r...
-00000b60: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00000b70: 0000 0300 0000 4300 0001 730a 0000 0074  ......C...s....t
-00000b80: 0064 0164 028d 0153 0029 034e 7223 0000  .d.d...S.).Nr#..
-00000b90: 0072 1700 0000 2901 7210 0000 0072 1800  .r....).r....r..
-00000ba0: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00000bb0: 0072 1a00 0000 5900 0000 7306 0000 0000  .r....Y...s.....
-00000bc0: 0202 0102 ff7a 1949 6d6d 6564 6961 7465  .....z.Immediate
-00000bd0: 4f72 4361 6e63 656c 2e74 6f5f 6a73 6f6e  OrCancel.to_json
-00000be0: 721b 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00000bf0: 0000 0100 0000 0200 0000 4300 0001 7308  ..........C...s.
-00000c00: 0000 0064 0169 0069 0153 0029 024e 7223  ...d.i.i.S.).Nr#
-00000c10: 0000 0072 0c00 0000 7218 0000 0072 0c00  ...r....r....r..
-00000c20: 0000 720c 0000 0072 0d00 0000 721c 0000  ..r....r....r...
-00000c30: 005f 0000 0073 0400 0000 0003 04ff 7a1e  ._...s........z.
-00000c40: 496d 6d65 6469 6174 654f 7243 616e 6365  ImmediateOrCance
-00000c50: 6c2e 746f 5f65 6e63 6f64 6162 6c65 4e72  l.to_encodableNr
-00000c60: 1d00 0000 720c 0000 0072 0c00 0000 720c  ....r....r....r.
-00000c70: 0000 0072 0d00 0000 7223 0000 0054 0000  ...r....r#...T..
-00000c80: 0073 0c00 0000 0a02 0c01 0c02 0201 1005  .s..............
-00000c90: 0201 7223 0000 0063 0000 0000 0000 0000  ..r#...c........
-00000ca0: 0000 0000 0000 0000 0400 0000 4000 0001  ............@...
-00000cb0: 734a 0000 0065 005a 0164 005a 0255 0064  sJ...e.Z.d.Z.U.d
-00000cc0: 015a 0364 0265 0464 033c 0064 005a 0564  .Z.d.e.d.<.d.Z.d
-00000cd0: 0265 0464 043c 0065 0664 0564 069c 0164  .e.d.<.e.d.d...d
-00000ce0: 0764 0884 0483 015a 0765 0664 0964 069c  .d.....Z.e.d.d..
-00000cf0: 0164 0a64 0b84 0483 015a 0864 0c53 0029  .d.d.....Z.d.S.)
-00000d00: 0dda 0d50 6f73 744f 6e6c 7953 6c69 6465  ...PostOnlySlide
-00000d10: e904 0000 0072 1300 0000 7214 0000 0072  .....r....r....r
-00000d20: 0600 0000 7211 0000 0072 1500 0000 6301  ....r....r....c.
-00000d30: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00000d40: 0000 0043 0000 0173 0a00 0000 7400 6401  ...C...s....t.d.
-00000d50: 6402 8d01 5300 2903 4e72 2500 0000 7217  d...S.).Nr%...r.
-00000d60: 0000 0029 0172 1100 0000 7218 0000 0072  ...).r....r....r
-00000d70: 0c00 0000 720c 0000 0072 0d00 0000 721a  ....r....r....r.
-00000d80: 0000 006b 0000 0073 0600 0000 0002 0201  ...k...s........
-00000d90: 02ff 7a15 506f 7374 4f6e 6c79 536c 6964  ..z.PostOnlySlid
-00000da0: 652e 746f 5f6a 736f 6e72 1b00 0000 6301  e.to_jsonr....c.
-00000db0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00000dc0: 0000 0043 0000 0173 0800 0000 6401 6900  ...C...s....d.i.
-00000dd0: 6901 5300 2902 4e72 2500 0000 720c 0000  i.S.).Nr%...r...
-00000de0: 0072 1800 0000 720c 0000 0072 0c00 0000  .r....r....r....
-00000df0: 720d 0000 0072 1c00 0000 7100 0000 7304  r....r....q...s.
-00000e00: 0000 0000 0304 ff7a 1a50 6f73 744f 6e6c  .......z.PostOnl
-00000e10: 7953 6c69 6465 2e74 6f5f 656e 636f 6461  ySlide.to_encoda
-00000e20: 626c 654e 721d 0000 0072 0c00 0000 720c  bleNr....r....r.
-00000e30: 0000 0072 0c00 0000 720d 0000 0072 2500  ...r....r....r%.
-00000e40: 0000 6600 0000 730c 0000 000a 020c 010c  ..f...s.........
-00000e50: 0202 0110 0502 0172 2500 0000 721b 0000  .......r%...r...
-00000e60: 00da 0d4f 7264 6572 5479 7065 4b69 6e64  ...OrderTypeKind
-00000e70: 2902 da03 6f62 6a72 1600 0000 6301 0000  )...objr....c...
-00000e80: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00000e90: 0043 0000 0173 6400 0000 7400 7c00 7401  .C...sd...t.|.t.
-00000ea0: 8302 7312 7402 6401 8301 8201 6402 7c00  ..s.t.d.....d.|.
-00000eb0: 7600 7220 7403 8300 5300 6403 7c00 7600  v.r t...S.d.|.v.
-00000ec0: 722e 7404 8300 5300 6404 7c00 7600 723c  r.t...S.d.|.v.r<
-00000ed0: 7405 8300 5300 6405 7c00 7600 724a 7406  t...S.d.|.v.rJt.
-00000ee0: 8300 5300 6406 7c00 7600 7258 7407 8300  ..S.d.|.v.rXt...
-00000ef0: 5300 7402 6401 8301 8201 6400 5300 2907  S.t.d.....d.S.).
-00000f00: 4e7a 1349 6e76 616c 6964 2065 6e75 6d20  Nz.Invalid enum 
-00000f10: 6f62 6a65 6374 7212 0000 0072 1f00 0000  objectr....r....
-00000f20: 7221 0000 0072 2300 0000 7225 0000 0029  r!...r#...r%...)
-00000f30: 08da 0a69 7369 6e73 7461 6e63 6572 1b00  ...isinstancer..
-00000f40: 0000 da0a 5661 6c75 6545 7272 6f72 7212  ....ValueErrorr.
-00000f50: 0000 0072 1f00 0000 7221 0000 0072 2300  ...r....r!...r#.
-00000f60: 0000 7225 0000 0029 0172 2800 0000 720c  ..r%...).r(...r.
-00000f70: 0000 0072 0c00 0000 720d 0000 00da 0c66  ...r....r......f
-00000f80: 726f 6d5f 6465 636f 6465 647c 0000 0073  rom_decoded|...s
-00000f90: 1a00 0000 0001 0a01 0801 0801 0601 0801  ................
-00000fa0: 0601 0801 0601 0801 0601 0801 0601 722b  ..............r+
-00000fb0: 0000 00da 0d4f 7264 6572 5479 7065 4a53  .....OrderTypeJS
-00000fc0: 4f4e 6301 0000 0000 0000 0000 0000 0002  ONc.............
-00000fd0: 0000 0003 0000 0043 0000 0173 7400 0000  .......C...st...
-00000fe0: 7c00 6401 1900 6402 6b02 7212 7400 8300  |.d...d.k.r.t...
-00000ff0: 5300 7c00 6401 1900 6403 6b02 7224 7401  S.|.d...d.k.r$t.
-00001000: 8300 5300 7c00 6401 1900 6404 6b02 7236  ..S.|.d...d.k.r6
-00001010: 7402 8300 5300 7c00 6401 1900 6405 6b02  t...S.|.d...d.k.
-00001020: 7248 7403 8300 5300 7c00 6401 1900 6406  rHt...S.|.d...d.
-00001030: 6b02 725a 7404 8300 5300 7c00 6401 1900  k.rZt...S.|.d...
-00001040: 7d01 7405 6407 7c01 9b00 9d02 8301 8201  }.t.d.|.........
-00001050: 6400 5300 2908 4e72 0600 0000 7212 0000  d.S.).Nr....r...
-00001060: 0072 1f00 0000 7221 0000 0072 2300 0000  .r....r!...r#...
-00001070: 7225 0000 007a 1855 6e72 6563 6f67 6e69  r%...z.Unrecogni
-00001080: 7a65 6420 656e 756d 206b 696e 643a 2029  zed enum kind: )
-00001090: 0672 1200 0000 721f 0000 0072 2100 0000  .r....r....r!...
-000010a0: 7223 0000 0072 2500 0000 722a 0000 0029  r#...r%...r*...)
-000010b0: 0272 2800 0000 7206 0000 0072 0c00 0000  .r(...r....r....
-000010c0: 720c 0000 0072 0d00 0000 da09 6672 6f6d  r....r......from
-000010d0: 5f6a 736f 6e8c 0000 0073 1800 0000 0001  _json....s......
-000010e0: 0c01 0601 0c01 0601 0c01 0601 0c01 0601  ................
-000010f0: 0c01 0601 0801 722d 0000 0029 1bda 0a5f  ......r-...)..._
-00001100: 5f66 7574 7572 655f 5f72 0200 0000 da06  _future__r......
-00001110: 7479 7069 6e67 da0b 6461 7461 636c 6173  typing..dataclas
-00001120: 7365 7372 0300 0000 da0f 626f 7273 685f  sesr......borsh_
-00001130: 636f 6e73 7472 7563 74da 0562 6f72 7368  construct..borsh
-00001140: da18 616e 6368 6f72 7079 2e62 6f72 7368  ..anchorpy.borsh
-00001150: 5f65 7874 656e 7369 6f6e 7204 0000 00da  _extensionr.....
-00001160: 0954 7970 6564 4469 6374 7205 0000 0072  .TypedDictr....r
-00001170: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
-00001180: 0000 0072 1200 0000 721f 0000 0072 2100  ...r....r....r!.
-00001190: 0000 7223 0000 0072 2500 0000 da05 556e  ..r#...r%.....Un
-000011a0: 696f 6e72 2700 0000 722c 0000 0072 2b00  ionr'...r,...r+.
-000011b0: 0000 722d 0000 00da 0743 5374 7275 6374  ..r-.....CStruct
-000011c0: da06 6c61 796f 7574 720c 0000 0072 0c00  ..layoutr....r..
-000011d0: 0000 720c 0000 0072 0d00 0000 da08 3c6d  ..r....r......<m
-000011e0: 6f64 756c 653e 0100 0000 733c 0000 000c  odule>....s<....
-000011f0: 0208 010c 0208 010c 0312 0412 0412 0412  ................
-00001200: 0412 0402 0110 1102 0110 1102 0110 1102  ................
-00001210: 0110 1102 0110 1114 0114 0310 1010 0f02  ................
-00001220: 010a 010a 010a 010a 010a fb              ...........
+00000200: 6403 5300 2904 da0d 556e 6465 6669 6e65  d.S.)...Undefine
+00000210: 644a 534f 4e7a 1b74 7970 696e 672e 4c69  dJSONz.typing.Li
+00000220: 7465 7261 6c5b 2755 6e64 6566 696e 6564  teral['Undefined
+00000230: 275d da04 6b69 6e64 4ea9 04da 085f 5f6e  ']..kindN....__n
+00000240: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000250: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00000260: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
+00000270: a900 720c 0000 0072 0c00 0000 fa59 2f55  ..r....r.....Y/U
+00000280: 7365 7273 2f74 6672 697a 7a61 2f44 6f63  sers/tfrizza/Doc
+00000290: 756d 656e 7473 2f7a 6574 612f 7a65 7461  uments/zeta/zeta
+000002a0: 2d70 792f 7a65 7461 5f70 792f 7a65 7461  -py/zeta_py/zeta
+000002b0: 5f63 6c69 656e 742f 7479 7065 732f 7472  _client/types/tr
+000002c0: 6561 7375 7279 5f6d 6f76 656d 656e 745f  easury_movement_
+000002d0: 7479 7065 2e70 7972 0500 0000 0a00 0000  type.pyr........
+000002e0: 7302 0000 000a 0172 0500 0000 6300 0000  s......r....c...
+000002f0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00000300: 0040 0000 0173 1600 0000 6500 5a01 6400  .@...s....e.Z.d.
+00000310: 5a02 5500 6401 6503 6402 3c00 6403 5300  Z.U.d.e.d.<.d.S.
+00000320: 2904 da1b 546f 5472 6561 7375 7279 4672  )...ToTreasuryFr
+00000330: 6f6d 496e 7375 7261 6e63 654a 534f 4e7a  omInsuranceJSONz
+00000340: 2974 7970 696e 672e 4c69 7465 7261 6c5b  )typing.Literal[
+00000350: 2754 6f54 7265 6173 7572 7946 726f 6d49  'ToTreasuryFromI
+00000360: 6e73 7572 616e 6365 275d 7206 0000 004e  nsurance']r....N
+00000370: 7207 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+00000380: 0c00 0000 720d 0000 0072 0e00 0000 0e00  ....r....r......
+00000390: 0000 7302 0000 000a 0172 0e00 0000 6300  ..s......r....c.
+000003a0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+000003b0: 0000 0040 0000 0173 1600 0000 6500 5a01  ...@...s....e.Z.
+000003c0: 6400 5a02 5500 6401 6503 6402 3c00 6403  d.Z.U.d.e.d.<.d.
+000003d0: 5300 2904 da1b 546f 496e 7375 7261 6e63  S.)...ToInsuranc
+000003e0: 6546 726f 6d54 7265 6173 7572 794a 534f  eFromTreasuryJSO
+000003f0: 4e7a 2974 7970 696e 672e 4c69 7465 7261  Nz)typing.Litera
+00000400: 6c5b 2754 6f49 6e73 7572 616e 6365 4672  l['ToInsuranceFr
+00000410: 6f6d 5472 6561 7375 7279 275d 7206 0000  omTreasury']r...
+00000420: 004e 7207 0000 0072 0c00 0000 720c 0000  .Nr....r....r...
+00000430: 0072 0c00 0000 720d 0000 0072 0f00 0000  .r....r....r....
+00000440: 1200 0000 7302 0000 000a 0172 0f00 0000  ....s......r....
+00000450: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000460: 0003 0000 0040 0000 0173 1600 0000 6500  .....@...s....e.
+00000470: 5a01 6400 5a02 5500 6401 6503 6402 3c00  Z.d.Z.U.d.e.d.<.
+00000480: 6403 5300 2904 da22 546f 5472 6561 7375  d.S.).."ToTreasu
+00000490: 7279 4672 6f6d 5265 6665 7272 616c 7352  ryFromReferralsR
+000004a0: 6577 6172 6473 4a53 4f4e 7a30 7479 7069  ewardsJSONz0typi
+000004b0: 6e67 2e4c 6974 6572 616c 5b27 546f 5472  ng.Literal['ToTr
+000004c0: 6561 7375 7279 4672 6f6d 5265 6665 7272  easuryFromReferr
+000004d0: 616c 7352 6577 6172 6473 275d 7206 0000  alsRewards']r...
+000004e0: 004e 7207 0000 0072 0c00 0000 720c 0000  .Nr....r....r...
+000004f0: 0072 0c00 0000 720d 0000 0072 1000 0000  .r....r....r....
+00000500: 1600 0000 7302 0000 000a 0172 1000 0000  ....s......r....
+00000510: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000520: 0003 0000 0040 0000 0173 1600 0000 6500  .....@...s....e.
+00000530: 5a01 6400 5a02 5500 6401 6503 6402 3c00  Z.d.Z.U.d.e.d.<.
+00000540: 6403 5300 2904 da22 546f 5265 6665 7272  d.S.).."ToReferr
+00000550: 616c 7352 6577 6172 6473 4672 6f6d 5472  alsRewardsFromTr
+00000560: 6561 7375 7279 4a53 4f4e 7a30 7479 7069  easuryJSONz0typi
+00000570: 6e67 2e4c 6974 6572 616c 5b27 546f 5265  ng.Literal['ToRe
+00000580: 6665 7272 616c 7352 6577 6172 6473 4672  ferralsRewardsFr
+00000590: 6f6d 5472 6561 7375 7279 275d 7206 0000  omTreasury']r...
+000005a0: 004e 7207 0000 0072 0c00 0000 720c 0000  .Nr....r....r...
+000005b0: 0072 0c00 0000 720d 0000 0072 1100 0000  .r....r....r....
+000005c0: 1a00 0000 7302 0000 000a 0172 1100 0000  ....s......r....
+000005d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000005e0: 0004 0000 0040 0000 0173 4a00 0000 6500  .....@...sJ...e.
+000005f0: 5a01 6400 5a02 5500 6401 5a03 6402 6504  Z.d.Z.U.d.Z.d.e.
+00000600: 6403 3c00 6400 5a05 6402 6504 6404 3c00  d.<.d.Z.d.e.d.<.
+00000610: 6506 6405 6406 9c01 6407 6408 8404 8301  e.d.d...d.d.....
+00000620: 5a07 6506 6409 6406 9c01 640a 640b 8404  Z.e.d.d...d.d...
+00000630: 8301 5a08 640c 5300 290d da09 556e 6465  ..Z.d.S.)...Unde
+00000640: 6669 6e65 6472 0100 0000 fa0f 7479 7069  finedr......typi
+00000650: 6e67 2e43 6c61 7373 5661 72da 0d64 6973  ng.ClassVar..dis
+00000660: 6372 696d 696e 6174 6f72 7206 0000 0072  criminatorr....r
+00000670: 0500 0000 a901 da06 7265 7475 726e 6301  ........returnc.
+00000680: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00000690: 0000 0043 0000 0173 0a00 0000 7400 6401  ...C...s....t.d.
+000006a0: 6402 8d01 5300 2903 4e72 1200 0000 a901  d...S.).Nr......
+000006b0: 7206 0000 0029 0172 0500 0000 a901 da03  r....).r........
+000006c0: 636c 7372 0c00 0000 720c 0000 0072 0d00  clsr....r....r..
+000006d0: 0000 da07 746f 5f6a 736f 6e23 0000 0073  ....to_json#...s
+000006e0: 0600 0000 0002 0201 02ff 7a11 556e 6465  ..........z.Unde
+000006f0: 6669 6e65 642e 746f 5f6a 736f 6eda 0464  fined.to_json..d
+00000700: 6963 7463 0100 0000 0000 0000 0000 0000  ictc............
+00000710: 0100 0000 0200 0000 4300 0001 7308 0000  ........C...s...
+00000720: 0064 0169 0069 0153 0029 024e 7212 0000  .d.i.i.S.).Nr...
+00000730: 0072 0c00 0000 7218 0000 0072 0c00 0000  .r....r....r....
+00000740: 720c 0000 0072 0d00 0000 da0c 746f 5f65  r....r......to_e
+00000750: 6e63 6f64 6162 6c65 2900 0000 7304 0000  ncodable)...s...
+00000760: 0000 0304 ff7a 1655 6e64 6566 696e 6564  .....z.Undefined
+00000770: 2e74 6f5f 656e 636f 6461 626c 654e a909  .to_encodableN..
+00000780: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00000790: 1400 0000 720b 0000 0072 0600 0000 da0b  ....r....r......
+000007a0: 636c 6173 736d 6574 686f 6472 1a00 0000  classmethodr....
+000007b0: 721c 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+000007c0: 0c00 0000 720d 0000 0072 1200 0000 1e00  ....r....r......
+000007d0: 0000 730c 0000 000a 020c 010c 0202 0110  ..s.............
+000007e0: 0502 0172 1200 0000 6300 0000 0000 0000  ...r....c.......
+000007f0: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
+00000800: 0173 4a00 0000 6500 5a01 6400 5a02 5500  .sJ...e.Z.d.Z.U.
+00000810: 6401 5a03 6402 6504 6403 3c00 6400 5a05  d.Z.d.e.d.<.d.Z.
+00000820: 6402 6504 6404 3c00 6506 6405 6406 9c01  d.e.d.<.e.d.d...
+00000830: 6407 6408 8404 8301 5a07 6506 6409 6406  d.d.....Z.e.d.d.
+00000840: 9c01 640a 640b 8404 8301 5a08 640c 5300  ..d.d.....Z.d.S.
+00000850: 290d da17 546f 5472 6561 7375 7279 4672  )...ToTreasuryFr
+00000860: 6f6d 496e 7375 7261 6e63 65e9 0100 0000  omInsurance.....
+00000870: 7213 0000 0072 1400 0000 7206 0000 0072  r....r....r....r
+00000880: 0e00 0000 7215 0000 0063 0100 0000 0000  ....r....c......
+00000890: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+000008a0: 0001 730a 0000 0074 0064 0164 028d 0153  ..s....t.d.d...S
+000008b0: 0029 034e 721f 0000 0072 1700 0000 2901  .).Nr....r....).
+000008c0: 720e 0000 0072 1800 0000 720c 0000 0072  r....r....r....r
+000008d0: 0c00 0000 720d 0000 0072 1a00 0000 3500  ....r....r....5.
+000008e0: 0000 7306 0000 0000 0202 0102 ff7a 1f54  ..s..........z.T
+000008f0: 6f54 7265 6173 7572 7946 726f 6d49 6e73  oTreasuryFromIns
+00000900: 7572 616e 6365 2e74 6f5f 6a73 6f6e 721b  urance.to_jsonr.
+00000910: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000920: 0100 0000 0200 0000 4300 0001 7308 0000  ........C...s...
+00000930: 0064 0169 0069 0153 0029 024e 721f 0000  .d.i.i.S.).Nr...
+00000940: 0072 0c00 0000 7218 0000 0072 0c00 0000  .r....r....r....
+00000950: 720c 0000 0072 0d00 0000 721c 0000 003b  r....r....r....;
+00000960: 0000 0073 0400 0000 0003 04ff 7a24 546f  ...s........z$To
+00000970: 5472 6561 7375 7279 4672 6f6d 496e 7375  TreasuryFromInsu
+00000980: 7261 6e63 652e 746f 5f65 6e63 6f64 6162  rance.to_encodab
+00000990: 6c65 4e72 1d00 0000 720c 0000 0072 0c00  leNr....r....r..
+000009a0: 0000 720c 0000 0072 0d00 0000 721f 0000  ..r....r....r...
+000009b0: 0030 0000 0073 0c00 0000 0a02 0c01 0c02  .0...s..........
+000009c0: 0201 1005 0201 721f 0000 0063 0000 0000  ......r....c....
+000009d0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+000009e0: 4000 0001 734a 0000 0065 005a 0164 005a  @...sJ...e.Z.d.Z
+000009f0: 0255 0064 015a 0364 0265 0464 033c 0064  .U.d.Z.d.e.d.<.d
+00000a00: 005a 0564 0265 0464 043c 0065 0664 0564  .Z.d.e.d.<.e.d.d
+00000a10: 069c 0164 0764 0884 0483 015a 0765 0664  ...d.d.....Z.e.d
+00000a20: 0964 069c 0164 0a64 0b84 0483 015a 0864  .d...d.d.....Z.d
+00000a30: 0c53 0029 0dda 1754 6f49 6e73 7572 616e  .S.)...ToInsuran
+00000a40: 6365 4672 6f6d 5472 6561 7375 7279 e902  ceFromTreasury..
+00000a50: 0000 0072 1300 0000 7214 0000 0072 0600  ...r....r....r..
+00000a60: 0000 720f 0000 0072 1500 0000 6301 0000  ..r....r....c...
+00000a70: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00000a80: 0043 0000 0173 0a00 0000 7400 6401 6402  .C...s....t.d.d.
+00000a90: 8d01 5300 2903 4e72 2100 0000 7217 0000  ..S.).Nr!...r...
+00000aa0: 0029 0172 0f00 0000 7218 0000 0072 0c00  .).r....r....r..
+00000ab0: 0000 720c 0000 0072 0d00 0000 721a 0000  ..r....r....r...
+00000ac0: 0047 0000 0073 0600 0000 0002 0201 02ff  .G...s..........
+00000ad0: 7a1f 546f 496e 7375 7261 6e63 6546 726f  z.ToInsuranceFro
+00000ae0: 6d54 7265 6173 7572 792e 746f 5f6a 736f  mTreasury.to_jso
+00000af0: 6e72 1b00 0000 6301 0000 0000 0000 0000  nr....c.........
+00000b00: 0000 0001 0000 0002 0000 0043 0000 0173  ...........C...s
+00000b10: 0800 0000 6401 6900 6901 5300 2902 4e72  ....d.i.i.S.).Nr
+00000b20: 2100 0000 720c 0000 0072 1800 0000 720c  !...r....r....r.
+00000b30: 0000 0072 0c00 0000 720d 0000 0072 1c00  ...r....r....r..
+00000b40: 0000 4d00 0000 7304 0000 0000 0304 ff7a  ..M...s........z
+00000b50: 2454 6f49 6e73 7572 616e 6365 4672 6f6d  $ToInsuranceFrom
+00000b60: 5472 6561 7375 7279 2e74 6f5f 656e 636f  Treasury.to_enco
+00000b70: 6461 626c 654e 721d 0000 0072 0c00 0000  dableNr....r....
+00000b80: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+00000b90: 2100 0000 4200 0000 730c 0000 000a 020c  !...B...s.......
+00000ba0: 010c 0202 0110 0502 0172 2100 0000 6300  .........r!...c.
+00000bb0: 0000 0000 0000 0000 0000 0000 0000 0004  ................
+00000bc0: 0000 0040 0000 0173 4a00 0000 6500 5a01  ...@...sJ...e.Z.
+00000bd0: 6400 5a02 5500 6401 5a03 6402 6504 6403  d.Z.U.d.Z.d.e.d.
+00000be0: 3c00 6400 5a05 6402 6504 6404 3c00 6506  <.d.Z.d.e.d.<.e.
+00000bf0: 6405 6406 9c01 6407 6408 8404 8301 5a07  d.d...d.d.....Z.
+00000c00: 6506 6409 6406 9c01 640a 640b 8404 8301  e.d.d...d.d.....
+00000c10: 5a08 640c 5300 290d da1e 546f 5472 6561  Z.d.S.)...ToTrea
+00000c20: 7375 7279 4672 6f6d 5265 6665 7272 616c  suryFromReferral
+00000c30: 7352 6577 6172 6473 e903 0000 0072 1300  sRewards.....r..
+00000c40: 0000 7214 0000 0072 0600 0000 7210 0000  ..r....r....r...
+00000c50: 0072 1500 0000 6301 0000 0000 0000 0000  .r....c.........
+00000c60: 0000 0001 0000 0003 0000 0043 0000 0173  ...........C...s
+00000c70: 0a00 0000 7400 6401 6402 8d01 5300 2903  ....t.d.d...S.).
+00000c80: 4e72 2300 0000 7217 0000 0029 0172 1000  Nr#...r....).r..
+00000c90: 0000 7218 0000 0072 0c00 0000 720c 0000  ..r....r....r...
+00000ca0: 0072 0d00 0000 721a 0000 0059 0000 0073  .r....r....Y...s
+00000cb0: 0600 0000 0002 0201 02ff 7a26 546f 5472  ..........z&ToTr
+00000cc0: 6561 7375 7279 4672 6f6d 5265 6665 7272  easuryFromReferr
+00000cd0: 616c 7352 6577 6172 6473 2e74 6f5f 6a73  alsRewards.to_js
+00000ce0: 6f6e 721b 0000 0063 0100 0000 0000 0000  onr....c........
+00000cf0: 0000 0000 0100 0000 0200 0000 4300 0001  ............C...
+00000d00: 7308 0000 0064 0169 0069 0153 0029 024e  s....d.i.i.S.).N
+00000d10: 7223 0000 0072 0c00 0000 7218 0000 0072  r#...r....r....r
+00000d20: 0c00 0000 720c 0000 0072 0d00 0000 721c  ....r....r....r.
+00000d30: 0000 005f 0000 0073 0400 0000 0003 04ff  ..._...s........
+00000d40: 7a2b 546f 5472 6561 7375 7279 4672 6f6d  z+ToTreasuryFrom
+00000d50: 5265 6665 7272 616c 7352 6577 6172 6473  ReferralsRewards
+00000d60: 2e74 6f5f 656e 636f 6461 626c 654e 721d  .to_encodableNr.
+00000d70: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
+00000d80: 0000 720d 0000 0072 2300 0000 5400 0000  ..r....r#...T...
+00000d90: 730c 0000 000a 020c 010c 0202 0110 0502  s...............
+00000da0: 0172 2300 0000 6300 0000 0000 0000 0000  .r#...c.........
+00000db0: 0000 0000 0000 0004 0000 0040 0000 0173  ...........@...s
+00000dc0: 4a00 0000 6500 5a01 6400 5a02 5500 6401  J...e.Z.d.Z.U.d.
+00000dd0: 5a03 6402 6504 6403 3c00 6400 5a05 6402  Z.d.e.d.<.d.Z.d.
+00000de0: 6504 6404 3c00 6506 6405 6406 9c01 6407  e.d.<.e.d.d...d.
+00000df0: 6408 8404 8301 5a07 6506 6409 6406 9c01  d.....Z.e.d.d...
+00000e00: 640a 640b 8404 8301 5a08 640c 5300 290d  d.d.....Z.d.S.).
+00000e10: da1e 546f 5265 6665 7272 616c 7352 6577  ..ToReferralsRew
+00000e20: 6172 6473 4672 6f6d 5472 6561 7375 7279  ardsFromTreasury
+00000e30: e904 0000 0072 1300 0000 7214 0000 0072  .....r....r....r
+00000e40: 0600 0000 7211 0000 0072 1500 0000 6301  ....r....r....c.
+00000e50: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00000e60: 0000 0043 0000 0173 0a00 0000 7400 6401  ...C...s....t.d.
+00000e70: 6402 8d01 5300 2903 4e72 2500 0000 7217  d...S.).Nr%...r.
+00000e80: 0000 0029 0172 1100 0000 7218 0000 0072  ...).r....r....r
+00000e90: 0c00 0000 720c 0000 0072 0d00 0000 721a  ....r....r....r.
+00000ea0: 0000 006b 0000 0073 0600 0000 0002 0201  ...k...s........
+00000eb0: 02ff 7a26 546f 5265 6665 7272 616c 7352  ..z&ToReferralsR
+00000ec0: 6577 6172 6473 4672 6f6d 5472 6561 7375  ewardsFromTreasu
+00000ed0: 7279 2e74 6f5f 6a73 6f6e 721b 0000 0063  ry.to_jsonr....c
+00000ee0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000ef0: 0200 0000 4300 0001 7308 0000 0064 0169  ....C...s....d.i
+00000f00: 0069 0153 0029 024e 7225 0000 0072 0c00  .i.S.).Nr%...r..
+00000f10: 0000 7218 0000 0072 0c00 0000 720c 0000  ..r....r....r...
+00000f20: 0072 0d00 0000 721c 0000 0071 0000 0073  .r....r....q...s
+00000f30: 0400 0000 0003 04ff 7a2b 546f 5265 6665  ........z+ToRefe
+00000f40: 7272 616c 7352 6577 6172 6473 4672 6f6d  rralsRewardsFrom
+00000f50: 5472 6561 7375 7279 2e74 6f5f 656e 636f  Treasury.to_enco
+00000f60: 6461 626c 654e 721d 0000 0072 0c00 0000  dableNr....r....
+00000f70: 720c 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+00000f80: 2500 0000 6600 0000 730c 0000 000a 020c  %...f...s.......
+00000f90: 010c 0202 0110 0502 0172 2500 0000 721b  .........r%...r.
+00000fa0: 0000 00da 1854 7265 6173 7572 794d 6f76  .....TreasuryMov
+00000fb0: 656d 656e 7454 7970 654b 696e 6429 02da  ementTypeKind)..
+00000fc0: 036f 626a 7216 0000 0063 0100 0000 0000  .objr....c......
+00000fd0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00000fe0: 0001 7364 0000 0074 007c 0074 0183 0273  ..sd...t.|.t...s
+00000ff0: 1274 0264 0183 0182 0164 027c 0076 0072  .t.d.....d.|.v.r
+00001000: 2074 0383 0053 0064 037c 0076 0072 2e74   t...S.d.|.v.r.t
+00001010: 0483 0053 0064 047c 0076 0072 3c74 0583  ...S.d.|.v.r<t..
+00001020: 0053 0064 057c 0076 0072 4a74 0683 0053  .S.d.|.v.rJt...S
+00001030: 0064 067c 0076 0072 5874 0783 0053 0074  .d.|.v.rXt...S.t
+00001040: 0264 0183 0182 0164 0053 0029 074e 7a13  .d.....d.S.).Nz.
+00001050: 496e 7661 6c69 6420 656e 756d 206f 626a  Invalid enum obj
+00001060: 6563 7472 1200 0000 721f 0000 0072 2100  ectr....r....r!.
+00001070: 0000 7223 0000 0072 2500 0000 2908 da0a  ..r#...r%...)...
+00001080: 6973 696e 7374 616e 6365 721b 0000 00da  isinstancer.....
+00001090: 0a56 616c 7565 4572 726f 7272 1200 0000  .ValueErrorr....
+000010a0: 721f 0000 0072 2100 0000 7223 0000 0072  r....r!...r#...r
+000010b0: 2500 0000 2901 7228 0000 0072 0c00 0000  %...).r(...r....
+000010c0: 720c 0000 0072 0d00 0000 da0c 6672 6f6d  r....r......from
+000010d0: 5f64 6563 6f64 6564 8800 0000 731a 0000  _decoded....s...
+000010e0: 0000 010a 0108 0108 0106 0108 0106 0108  ................
+000010f0: 0106 0108 0106 0108 0106 0172 2b00 0000  ...........r+...
+00001100: da18 5472 6561 7375 7279 4d6f 7665 6d65  ..TreasuryMoveme
+00001110: 6e74 5479 7065 4a53 4f4e 6301 0000 0000  ntTypeJSONc.....
+00001120: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00001130: 0000 0173 7400 0000 7c00 6401 1900 6402  ...st...|.d...d.
+00001140: 6b02 7212 7400 8300 5300 7c00 6401 1900  k.r.t...S.|.d...
+00001150: 6403 6b02 7224 7401 8300 5300 7c00 6401  d.k.r$t...S.|.d.
+00001160: 1900 6404 6b02 7236 7402 8300 5300 7c00  ..d.k.r6t...S.|.
+00001170: 6401 1900 6405 6b02 7248 7403 8300 5300  d...d.k.rHt...S.
+00001180: 7c00 6401 1900 6406 6b02 725a 7404 8300  |.d...d.k.rZt...
+00001190: 5300 7c00 6401 1900 7d01 7405 6407 7c01  S.|.d...}.t.d.|.
+000011a0: 9b00 9d02 8301 8201 6400 5300 2908 4e72  ........d.S.).Nr
+000011b0: 0600 0000 7212 0000 0072 1f00 0000 7221  ....r....r....r!
+000011c0: 0000 0072 2300 0000 7225 0000 007a 1855  ...r#...r%...z.U
+000011d0: 6e72 6563 6f67 6e69 7a65 6420 656e 756d  nrecognized enum
+000011e0: 206b 696e 643a 2029 0672 1200 0000 721f   kind: ).r....r.
+000011f0: 0000 0072 2100 0000 7223 0000 0072 2500  ...r!...r#...r%.
+00001200: 0000 722a 0000 0029 0272 2800 0000 7206  ..r*...).r(...r.
+00001210: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+00001220: 0000 da09 6672 6f6d 5f6a 736f 6e98 0000  ....from_json...
+00001230: 0073 1800 0000 0001 0c01 0601 0c01 0601  .s..............
+00001240: 0c01 0601 0c01 0601 0c01 0601 0801 722d  ..............r-
+00001250: 0000 0029 1bda 0a5f 5f66 7574 7572 655f  ...)...__future_
+00001260: 5f72 0200 0000 da06 7479 7069 6e67 da0b  _r......typing..
+00001270: 6461 7461 636c 6173 7365 7372 0300 0000  dataclassesr....
+00001280: da0f 626f 7273 685f 636f 6e73 7472 7563  ..borsh_construc
+00001290: 74da 0562 6f72 7368 da18 616e 6368 6f72  t..borsh..anchor
+000012a0: 7079 2e62 6f72 7368 5f65 7874 656e 7369  py.borsh_extensi
+000012b0: 6f6e 7204 0000 00da 0954 7970 6564 4469  onr......TypedDi
+000012c0: 6374 7205 0000 0072 0e00 0000 720f 0000  ctr....r....r...
+000012d0: 0072 1000 0000 7211 0000 0072 1200 0000  .r....r....r....
+000012e0: 721f 0000 0072 2100 0000 7223 0000 0072  r....r!...r#...r
+000012f0: 2500 0000 da05 556e 696f 6e72 2700 0000  %.....Unionr'...
+00001300: 722c 0000 0072 2b00 0000 722d 0000 00da  r,...r+...r-....
+00001310: 0743 5374 7275 6374 da06 6c61 796f 7574  .CStruct..layout
+00001320: 720c 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+00001330: 0d00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00001340: 0000 7358 0000 000c 0208 010c 0208 010c  ..sX............
+00001350: 0312 0412 0412 0412 0412 0402 0110 1102  ................
+00001360: 0110 1102 0110 1102 0110 1102 0110 1104  ................
+00001370: 0102 0102 0102 0102 0102 fc02 ff04 0704  ................
+00001380: 0102 0102 0102 0102 0102 fc02 ff04 0910  ................
+00001390: 1010 0f02 010a 010a 010a 010a 010a fb    ...............
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/override_expiry_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/override_expiry_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/override_expiry_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/override_expiry_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/perp_parameters.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/perp_parameters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/perp_parameters.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/perp_parameters.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/place_order_type.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/place_order_type.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/place_order_type.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/place_order_type.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/position.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/position.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/position.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/position.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/position_movement_arg.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/position_movement_arg.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/position_movement_arg.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/position_movement_arg.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/pricing_parameters.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/pricing_parameters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/pricing_parameters.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/pricing_parameters.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/product.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/product.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/product.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/product.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/product_greeks.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/product_greeks.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/product_greeks.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/product_greeks.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/product_ledger.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/product_ledger.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/product_ledger.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/product_ledger.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/set_referrals_rewards_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/set_referrals_rewards_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/set_referrals_rewards_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/set_referrals_rewards_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/side.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/side.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/side.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/side.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/strike.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/strike.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/strike.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/strike.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/trait_type.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/trait_type.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/trait_type.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/trait_type.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/treasury_movement_type.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/treasury_movement_type.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_greeks_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_greeks_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_greeks_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_greeks_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_interest_rate_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_interest_rate_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_interest_rate_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_interest_rate_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_margin_parameters_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_margin_parameters_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_margin_parameters_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_margin_parameters_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_perp_parameters_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_perp_parameters_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_perp_parameters_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_perp_parameters_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_pricing_parameters_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_pricing_parameters_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_pricing_parameters_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_pricing_parameters_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_state_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_state_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_state_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_state_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_volatility_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_volatility_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_volatility_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_volatility_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_zeta_group_expiry_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_zeta_group_expiry_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_zeta_group_expiry_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_zeta_group_expiry_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_zeta_pricing_pubkeys_args.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_zeta_pricing_pubkeys_args.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/update_zeta_pricing_pubkeys_args.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/update_zeta_pricing_pubkeys_args.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/validation_type.cpython-311.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/validation_type.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/__pycache__/validation_type.cpython-39.pyc` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/__pycache__/validation_type.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/anchor_decimal.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/anchor_decimal.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/asset.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/asset.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,18 @@
     kind: typing.Literal["ARB"]
 
 
 class BNBJSON(typing.TypedDict):
     kind: typing.Literal["BNB"]
 
 
+class PYTHJSON(typing.TypedDict):
+    kind: typing.Literal["PYTH"]
+
+
 class UNDEFINEDJSON(typing.TypedDict):
     kind: typing.Literal["UNDEFINED"]
 
 
 @dataclass
 class SOL:
     discriminator: typing.ClassVar = 0
@@ -140,16 +144,34 @@
     def to_encodable(cls) -> dict:
         return {
             "BNB": {},
         }
 
 
 @dataclass
+class PYTH:
+    discriminator: typing.ClassVar = 6
+    kind: typing.ClassVar = "PYTH"
+
+    @classmethod
+    def to_json(cls) -> PYTHJSON:
+        return PYTHJSON(
+            kind="PYTH",
+        )
+
+    @classmethod
+    def to_encodable(cls) -> dict:
+        return {
+            "PYTH": {},
+        }
+
+
+@dataclass
 class UNDEFINED:
-    discriminator: typing.ClassVar = 5
+    discriminator: typing.ClassVar = 7
     kind: typing.ClassVar = "UNDEFINED"
 
     @classmethod
     def to_json(cls) -> UNDEFINEDJSON:
         return UNDEFINEDJSON(
             kind="UNDEFINED",
         )
@@ -157,16 +179,16 @@
     @classmethod
     def to_encodable(cls) -> dict:
         return {
             "UNDEFINED": {},
         }
 
 
-AssetKind = typing.Union[SOL, BTC, ETH, APT, ARB, BNB, UNDEFINED]
-AssetJSON = typing.Union[SOLJSON, BTCJSON, ETHJSON, APTJSON, ARBJSON, BNBJSON, UNDEFINEDJSON]
+AssetKind = typing.Union[SOL, BTC, ETH, APT, ARB, BNB, PYTH, UNDEFINED]
+AssetJSON = typing.Union[SOLJSON, BTCJSON, ETHJSON, APTJSON, ARBJSON, BNBJSON, PYTHJSON, UNDEFINEDJSON]
 
 
 def from_decoded(obj: dict) -> AssetKind:
     if not isinstance(obj, dict):
         raise ValueError("Invalid enum object")
     if "SOL" in obj:
         return SOL()
@@ -176,14 +198,16 @@
         return ETH()
     if "APT" in obj:
         return APT()
     if "ARB" in obj:
         return ARB()
     if "BNB" in obj:
         return BNB()
+    if "PYTH" in obj:
+        return PYTH()
     if "UNDEFINED" in obj:
         return UNDEFINED()
     raise ValueError("Invalid enum object")
 
 
 def from_json(obj: AssetJSON) -> AssetKind:
     if obj["kind"] == "SOL":
@@ -194,22 +218,25 @@
         return ETH()
     if obj["kind"] == "APT":
         return APT()
     if obj["kind"] == "ARB":
         return ARB()
     if obj["kind"] == "BNB":
         return BNB()
+    if obj["kind"] == "PYTH":
+        return PYTH()
     if obj["kind"] == "UNDEFINED":
         return UNDEFINED()
     kind = obj["kind"]
     raise ValueError(f"Unrecognized enum kind: {kind}")
 
 
 layout = EnumForCodegen(
     "SOL" / borsh.CStruct(),
     "BTC" / borsh.CStruct(),
     "ETH" / borsh.CStruct(),
     "APT" / borsh.CStruct(),
     "ARB" / borsh.CStruct(),
     "BNB" / borsh.CStruct(),
+    "PYTH" / borsh.CStruct(),
     "UNDEFINED" / borsh.CStruct(),
 )
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/cross_margin_account_info.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/cross_margin_account_info.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/halt_args.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/halt_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class HaltArgsJSON(typing.TypedDict):
     spot_prices: list[int]
     timestamp: int
 
 
 @dataclass
 class HaltArgs:
-    layout: typing.ClassVar = borsh.CStruct("spot_prices" / borsh.U64[5], "timestamp" / borsh.U64)
+    layout: typing.ClassVar = borsh.CStruct("spot_prices" / borsh.U64[7], "timestamp" / borsh.U64)
     spot_prices: list[int]
     timestamp: int
 
     @classmethod
     def from_decoded(cls, obj: Container) -> "HaltArgs":
         return cls(spot_prices=obj.spot_prices, timestamp=obj.timestamp)
```

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/halt_state.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/halt_state.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/halt_state_args.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/halt_state_args.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/halt_state_v2.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/halt_state_v2.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/initialize_market_args.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/initialize_market_args.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/initialize_market_node_args.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/initialize_market_node_args.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/initialize_state_args.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/initialize_state_args.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/initialize_zeta_pricing_args.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/initialize_zeta_pricing_args.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/kind.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/kind.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/margin_account_type.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/margin_account_type.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/margin_parameters.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/margin_parameters.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/margin_requirement.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/margin_requirement.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/movement_type.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/movement_type.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/order_complete_type.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/order_complete_type.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/order_state.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/order_state.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/order_type.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/order_type.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/perp_parameters.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/perp_parameters.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/place_order_type.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/place_order_type.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/position.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/position.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/pricing_parameters.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/pricing_parameters.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/product.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/product.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/product_greeks.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/product_greeks.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/product_ledger.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/product_ledger.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/set_referrals_rewards_args.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/set_referrals_rewards_args.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/side.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/side.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/strike.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/strike.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/trait_type.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/trait_type.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/treasury_movement_type.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/treasury_movement_type.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/update_margin_parameters_args.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/update_margin_parameters_args.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/update_perp_parameters_args.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/update_perp_parameters_args.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/update_pricing_parameters_args.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/update_pricing_parameters_args.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/update_state_args.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/update_state_args.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/update_zeta_pricing_pubkeys_args.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/update_zeta_pricing_pubkeys_args.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/zetamarkets_py/zeta_client/types/validation_type.py` & `zetamarkets_py-0.2.9/zetamarkets_py/zeta_client/types/validation_type.py`

 * *Files identical despite different names*

### Comparing `zetamarkets_py-0.2.7/PKG-INFO` & `zetamarkets_py-0.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: zetamarkets-py
-Version: 0.2.7
+Version: 0.2.9
 Summary: Python SDK for Zeta Markets
 Home-page: https://github.com/zetamarkets/zetamarkets-py
 License: Apache-2.0
 Author: Tristan0x
 Author-email: tristan@sierra.team
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anchorpy (>=0.18.0,<0.19.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: deprecated (>=1.2.14,<2.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: solana (>=0.30.2,<0.31.0)
 Requires-Dist: solders (>=0.18.1,<0.19.0)
 Project-URL: Repository, https://github.com/zetamarkets/zetamarkets-py
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img height="120px" src="./logos/zeta-py.png" />
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: zetamarkets-py Version: 0.2.7 Summary: Python SDK
+Metadata-Version: 2.1 Name: zetamarkets-py Version: 0.2.9 Summary: Python SDK
 for Zeta Markets Home-page: https://github.com/zetamarkets/zetamarkets-py
 License: Apache-2.0 Author: Tristan0x Author-email: tristan@sierra.team
 Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: anchorpy (>=0.18.0,<0.19.0) Requires-Dist: colorlog (>=6.7.0,<7.0.0)
-Requires-Dist: deprecated (>=1.2.14,<2.0.0) Requires-Dist: requests
-(>=2.31.0,<3.0.0) Requires-Dist: solana (>=0.30.2,<0.31.0) Requires-Dist:
-solders (>=0.18.1,<0.19.0) Project-URL: Repository, https://github.com/
-zetamarkets/zetamarkets-py Description-Content-Type: text/markdown
+Requires-Dist: deprecated (>=1.2.14,<2.0.0) Requires-Dist: solana
+(>=0.30.2,<0.31.0) Requires-Dist: solders (>=0.18.1,<0.19.0) Project-URL:
+Repository, https://github.com/zetamarkets/zetamarkets-py Description-Content-
+Type: text/markdown
                              [./logos/zeta-py.png]
                       ************ ZZeettaa PPyytthhoonn SSDDKK ?ð??? ************
           _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]_[_D_i_s_c_o_r_d_ _C_h_a_t_]
 ## Installation ### Install from PyPI ```sh pip install zetamarkets_py ``` ###
 Install from Source You can add optional dependencies for running trading
 examples or docs using the `--with` flag. ```sh poetry install [--with
 examples, docs] ``` ## Usage ### Setting up a Solana wallet Please follow the
```

