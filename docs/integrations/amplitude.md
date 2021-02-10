description: Integrate Flagsmith with Datadog

# Amplitude Integration

<img src="/images/integrations/amplitude/amplitude-logo.svg"/>

!!! note
    This feature is currently in beta. Please contact us if you are interested in joining the beta!

You can integrate Flagsmith with Amplitude. You can automate AB tests by connecting the Flagsmith platform with Amplitude. The process is as follows:

## Integration Setup

1. Get the Amplitude API key for your Amplitude project from the Amplitude Project page (Settings > Projects > Your Project > General tab)
2. Add the Amplitude API key into Flagsmith (contact us for beta access to this!)
3. All API calls generated by the Flagsmith SDK to the `Get Identity Flags` endpoint will send the a full set of flag evaluations for that particular user to the Amplitude [`Identify` endpoint](https://developers.amplitude.com/docs/identify-api)

## Use Case

Once the integration has been set up, you can start segmenting your Amplitude identities based on the flags that they saw. This means you can run AB tests driven by Flagsmith segments, and have the data show up automatically in Amplitude. 

## Integration Notes

You have to identify users on both platforms in the same way. The Flagsmith `Identity ID` must be the same as the Amplitude `user_id`.