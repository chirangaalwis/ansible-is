# Continuous Update Delivery for WSO2 Identity Server

The update script is to be used by WSO2 subscription users such that products packs can be updated. If you do not have a WSO2 subscription, you can sign up for a [free trial](https://wso2.com/subscription/free-trial).

### Prequisites
* A WSO2 Subscription
* [WUM](https://wso2.com/updates/wum) updated packs should be provided in the `/files/packs` directory

`
NOTE: Provided WUM updated packs should contain the latest updates for wso2is-5.8.0 and wso2is-analytics-5.8.0
`

### Usage
While executing the update script, provide the profile name. The pack corresponding to the profile will begin updating.
```bash
./update.sh -p <profile-name>
```
Any of the following profile names can be provided as arguments:
* is
* is-analytics-dashboard
* is-analytics-worker

If any file that is used as a template is updated, a warning will be displayed. Update the relevant template files accordingly before pushing updates to the nodes.
