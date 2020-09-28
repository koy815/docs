---
title: Viewing job execution time
intro: 'You can view the execution time of a job, including the billable minutes that a job accrued.'
product: '{{ site.data.reusables.gated-features.actions }}'
versions:
  free-pro-team: '*'
---

{{ site.data.reusables.actions.enterprise-beta }}
{{ site.data.reusables.actions.enterprise-github-hosted-runners }}

Billable job execution minutes are only shown for jobs run on private repositories that use {{ site.data.variables.product.prodname_dotcom }}-hosted runners. There are no billable minutes when using {{ site.data.variables.product.prodname_actions }} in public repositories or for jobs run on self-hosted runners.

{{ site.data.reusables.repositories.navigate-to-repo }}
{{ site.data.reusables.repositories.actions-tab }}
{{ site.data.reusables.repositories.navigate-to-workflow }}
{{ site.data.reusables.repositories.view-run }}
1. Under the job summary, you can view the job's execution time. To view the billable job execution time, click **Run and billable time details**.
   ![Run and billable time details link](/assets/images/help/repository/view-run-billable-time.png)

   {% note %}
   
   **Note:** The billable time shown does not include any rounding or minute multipliers. To view your total {{ site.data.variables.product.prodname_actions }} usage, including rounding and minute multipliers, see "[Viewing your {{ site.data.variables.product.prodname_actions }} usage](/github/setting-up-and-managing-billing-and-payments-on-github/viewing-your-github-actions-usage)."
   
   {% endnote %}