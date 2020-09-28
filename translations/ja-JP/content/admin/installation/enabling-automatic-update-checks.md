---
title: 自動アップデートチェックの有効化
intro: '自動アップデートチェックを有効にすると、{{ site.data.variables.product.product_location_enterprise }} が最新の {{ site.data.variables.product.prodname_ghe_server }} リリースをチェックしてダウンロードします。'
redirect_from:
  - /enterprise/admin/installation/enabling-automatic-update-checks
versions:
  enterprise-server: '*'
---

{{ site.data.variables.product.product_location_enterprise }} のアップグレードパッケージが自動的にダウンロードされると、{{ site.data.variables.product.prodname_ghe_server }} をアップグレードできることを知らせるメッセージを受け取ります。 パッケージは{{ site.data.variables.product.product_location_enterprise }}の `/var/lib/ghe-updates`ディレクトリへダウンロードされます。 詳細は「[{{ site.data.variables.product.prodname_ghe_server }} をアップグレードする](/enterprise/{{ currentVersion }}/admin/guides/installation/upgrading-github-enterprise-server)」を参照してください。

アップグレードにホットパッチが利用できる場合、`.hpkg` は自動的にダウンロードします。 管理コンソールでは、ホットパッチを直ちにインストールするか、後でインストールするようにスケジュール設定するかを選択できます。 詳細は「[ホットパッチ付きでアップグレードする](/enterprise/{{ currentVersion }}/admin/guides/installation/upgrading-github-enterprise-server#upgrading-with-a-hotpatch)」を参照してください。

{% tip %}

**Tip:** 自動アップデートチェックを有効化するには、{{ site.data.variables.product.product_location_enterprise }}は`https://github-enterprise.s3.amazonaws.com`に接続できなければなりません。

{% endtip %}

{{ site.data.reusables.enterprise_site_admin_settings.access-settings }}
{{ site.data.reusables.enterprise_site_admin_settings.management-console }}
{{ site.data.reusables.enterprise_management_console.updates-tab }}
4. **Yes, automatically check for updates（はい、アップデートを自動的にチェックする）**をクリックしてください。 ![自動更新を有効化するためのボタン](/assets/images/enterprise/management-console/enable_updates_button.png)
{{ site.data.reusables.enterprise_management_console.save-settings }}

インスタンスが最新の状態になっているかを知るには、Updatesタブのバナーを調べてください。

![GitHub Enterprise Server のリリースを示すバナー](/assets/images/enterprise/management-console/up-to-date-banner.png)

**Logs（ログ）**の下で、最も直近のアップデートチェックのステータスを確認できます。

![アップデートのログ](/assets/images/enterprise/management-console/update-log.png)