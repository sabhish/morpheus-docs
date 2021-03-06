Guidance
========

Overview
--------

The `Operations -> Guidance` section shows recommendations for resource and costs utilization optimization. By analyzing the CPU, RAM, and Storage activity of Instances and Hosts, |morpheus| can recommend actions for Sizing and Power State.

Configuration
^^^^^^^^^^^^^^

Guidance is configured per Cloud and is set to off by default.

To turn on Guidance for a Cloud:

#. Navigate to `Infrastructure -> Clouds`.
#. Select the Edit icon of the Cloud to configure Guidance for.
#. Expand the `Advanced Options` section in the Edit Cloud modal.
#. In the *Guidance* dropdown, select Manual.
#. Select Save Changes.

Guidance recommendations will begin to appear in the guidance section when generated.

Once Guidance has been turned on for a cloud, Morpheus will determine if a guidance recommendation should be made once every 30 minutes. In the event that no recommendations can be made, no entry will be added to the list of suggested guidances. As the guidance list continues to grow, sorting and filtering may become necessary to focus on the recommendations that are relevant to the user at the time.

It's important to note that acting on recommendations is entirely manual at this time. In many cases, Morpheus provides one-click action to take the recommended steps but Guidance recommendations cannot be taken automatically. This is a feature that is being explored for a future update but has not been tagged for any specific release version at this time.

To see more detail on a Guidance recommendation in your list, click on the (i) button at the far right side of each list row. This will open a detail modal that gives additional information on the Guidance entry. In some cases, such as with sizing and shutdown recommendations, the user can simply click the "EXECUTE" button to take the recommended action as shown below.

.. image:: /images/operations/guidance/sizingexecute.png
  :width: 80%
  :alt: The execute button allows the user to immediately take action on a sizing recommendation
  :align: center

Other types of Guidance recommendations, such as reserve compute recommendations, must be taken in the cloud and Morpheus does not offer the execute button.

.. image:: /images/operations/guidance/reservecompute.png
  :width: 80%
  :alt: The execute button is not present on a reserve compute recommendation
  :align: center

Recommendations
^^^^^^^^^^^^^^^^^^

To view and act on Guidance recommendations, navigate to `Operations -> Guidance`.

The Guidance list contains the following details:

Severity Icon
  Indicates the severity of the recommended action.
Type
  Recommended action Type
Metric
  Guidance Metric used for recommended action.
Action
  Recommended Action for the Instance or Host, such as "Reduce Host memory" or "Shutdown Instance"
RESOURCE
  The Instance or Host targeted
SAVINGS
  Shows projected Monthly Costs savings if recommended action is taken.
DATE
  Date and Time stamp the recommended action was generated.
Information Link
  Click to view details on the recommendation.

.. NOTE:: Guidance Actions are not automatically triggered at this time.

Filters
^^^^^^^^^^

Search
  Search for Guidance recommendations
Type
  Filter by Sizing or Shutdown Guidance Types.
Severity
  Filter by Guidance Severity of All, Info, Warning, or Critical.
Metric
  Filter by All, Memory, CPU, or Power Guidance Metrics.
