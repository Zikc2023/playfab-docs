---
author: jasonsandlin
title: "Services C API overview - PFAccountManagementTypes.h"
description: "Services C API overview - PFAccountManagementTypes.h"
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 09/25/2023
---

# Services C API overview - PFAccountManagementTypes.h

  
## Structures  

| Structure | Description |  
| --- | --- |  
| [PFAccountManagementAddOrUpdateContactEmailRequest](structs/pfaccountmanagementaddorupdatecontactemailrequest.md) | PFAccountManagementAddOrUpdateContactEmailRequest data model. This API adds a contact email to the player's profile. If the player's profile already contains a contact email, it will update the contact email to the email address specified. |  
| [PFAccountManagementAddUsernamePasswordRequest](structs/pfaccountmanagementaddusernamepasswordrequest.md) | PFAccountManagementAddUsernamePasswordRequest data model. |  
| [PFAccountManagementAddUsernamePasswordResult](structs/pfaccountmanagementaddusernamepasswordresult.md) | PFAccountManagementAddUsernamePasswordResult data model. Each account must have a unique username and email address in the PlayFab service. Once created, the account may be associated with additional accounts (Steam, Facebook, Game Center, etc.), allowing for added social network lists and achievements systems. This can also be used to provide a recovery method if the user loses their original means of access. |  
| [PFAccountManagementBanInfo](structs/pfaccountmanagementbaninfo.md) | PFAccountManagementBanInfo data model. Contains information for a ban. |  
| [PFAccountManagementBanRequest](structs/pfaccountmanagementbanrequest.md) | PFAccountManagementBanRequest data model. Represents a single ban request. |  
| [PFAccountManagementBanUsersRequest](structs/pfaccountmanagementbanusersrequest.md) | PFAccountManagementBanUsersRequest data model. The existence of each user will not be verified. When banning by IP or MAC address, multiple players may be affected, so use this feature with caution. Returns information about the new bans. |  
| [PFAccountManagementBanUsersResult](structs/pfaccountmanagementbanusersresult.md) | PFAccountManagementBanUsersResult data model. |  
| [PFAccountManagementClientLinkNintendoServiceAccountRequest](structs/pfaccountmanagementclientlinknintendoserviceaccountrequest.md) | PFAccountManagementClientLinkNintendoServiceAccountRequest data model. |  
| [PFAccountManagementClientLinkNintendoSwitchDeviceIdRequest](structs/pfaccountmanagementclientlinknintendoswitchdeviceidrequest.md) | PFAccountManagementClientLinkNintendoSwitchDeviceIdRequest data model. |  
| [PFAccountManagementClientLinkPSNAccountRequest](structs/pfaccountmanagementclientlinkpsnaccountrequest.md) | PFAccountManagementClientLinkPSNAccountRequest data model. |  
| [PFAccountManagementClientLinkXboxAccountRequest](structs/pfaccountmanagementclientlinkxboxaccountrequest.md) | PFAccountManagementClientLinkXboxAccountRequest data model. |  
| [PFAccountManagementClientUnlinkNintendoServiceAccountRequest](structs/pfaccountmanagementclientunlinknintendoserviceaccountrequest.md) | PFAccountManagementClientUnlinkNintendoServiceAccountRequest data model. |  
| [PFAccountManagementClientUnlinkNintendoSwitchDeviceIdRequest](structs/pfaccountmanagementclientunlinknintendoswitchdeviceidrequest.md) | PFAccountManagementClientUnlinkNintendoSwitchDeviceIdRequest data model. |  
| [PFAccountManagementClientUnlinkPSNAccountRequest](structs/pfaccountmanagementclientunlinkpsnaccountrequest.md) | PFAccountManagementClientUnlinkPSNAccountRequest data model. |  
| [PFAccountManagementClientUnlinkXboxAccountRequest](structs/pfaccountmanagementclientunlinkxboxaccountrequest.md) | PFAccountManagementClientUnlinkXboxAccountRequest data model. |  
| [PFAccountManagementClientUpdateAvatarUrlRequest](structs/pfaccountmanagementclientupdateavatarurlrequest.md) | PFAccountManagementClientUpdateAvatarUrlRequest data model. |  
| [PFAccountManagementDeletePlayerRequest](structs/pfaccountmanagementdeleteplayerrequest.md) | PFAccountManagementDeletePlayerRequest data model. Deletes all data associated with the player, including statistics, custom data, inventory, purchases, virtual currency balances, characters and shared group memberships. Removes the player from all leaderboards and player search indexes. Does not delete PlayStream event history associated with the player. Does not delete the publisher user account that created the player in the title nor associated data such as username, password, email address, account linkages, or friends list. Note, this API queues the player for deletion and returns immediately. It may take several minutes or more before all player data is fully deleted. Until the player data is fully deleted, attempts to recreate the player with the same user account in the same title will fail with the 'AccountDeleted' error. This API must be enabled for use as an option in the game manager website. It is disabled by default. |  
| [PFAccountManagementFacebookInstantGamesPlayFabIdPair](structs/pfaccountmanagementfacebookinstantgamesplayfabidpair.md) | PFAccountManagementFacebookInstantGamesPlayFabIdPair data model. |  
| [PFAccountManagementFacebookPlayFabIdPair](structs/pfaccountmanagementfacebookplayfabidpair.md) | PFAccountManagementFacebookPlayFabIdPair data model. |  
| [PFAccountManagementGameCenterPlayFabIdPair](structs/pfaccountmanagementgamecenterplayfabidpair.md) | PFAccountManagementGameCenterPlayFabIdPair data model. |  
| [PFAccountManagementGetAccountInfoRequest](structs/pfaccountmanagementgetaccountinforequest.md) | PFAccountManagementGetAccountInfoRequest data model. |  
| [PFAccountManagementGetAccountInfoResult](structs/pfaccountmanagementgetaccountinforesult.md) | PFAccountManagementGetAccountInfoResult data model. This API retrieves details regarding the player in the PlayFab service. Note that when this call is used to retrieve data about another player (not the one signed into the local client), some data, such as Personally Identifying Information (PII), will be omitted for privacy reasons or to comply with the requirements of the platform belongs to. The user account returned will be based on the identifier provided in priority order: PlayFabId, Username, Email, then TitleDisplayName. If no identifier is specified, the currently signed in user's information will be returned. |  
| [PFAccountManagementGetPlayerCombinedInfoRequest](structs/pfaccountmanagementgetplayercombinedinforequest.md) | PFAccountManagementGetPlayerCombinedInfoRequest data model. |  
| [PFAccountManagementGetPlayerCombinedInfoResult](structs/pfaccountmanagementgetplayercombinedinforesult.md) | PFAccountManagementGetPlayerCombinedInfoResult data model. Returns whatever info is requested in the response for the user. If no user is explicitly requested this defaults to the authenticated user. If the user is the same as the requester, PII (like email address, facebook id) is returned if available. Otherwise, only public information is returned. All parameters default to false. |  
| [PFAccountManagementGetPlayerProfileRequest](structs/pfaccountmanagementgetplayerprofilerequest.md) | PFAccountManagementGetPlayerProfileRequest data model. This API allows for access to details regarding a user in the PlayFab service, usually for purposes of customer support. Note that data returned may be Personally Identifying Information (PII), such as email address, and so care should be taken in how this data is stored and managed. Since this call will always return the relevant information for users who have accessed the title, the recommendation is to not store this data locally. |  
| [PFAccountManagementGetPlayerProfileResult](structs/pfaccountmanagementgetplayerprofileresult.md) | PFAccountManagementGetPlayerProfileResult data model. |  
| [PFAccountManagementGetPlayFabIDsFromFacebookIDsRequest](structs/pfaccountmanagementgetplayfabidsfromfacebookidsrequest.md) | PFAccountManagementGetPlayFabIDsFromFacebookIDsRequest data model. |  
| [PFAccountManagementGetPlayFabIDsFromFacebookIDsResult](structs/pfaccountmanagementgetplayfabidsfromfacebookidsresult.md) | PFAccountManagementGetPlayFabIDsFromFacebookIDsResult data model. For Facebook identifiers which have not been linked to PlayFab accounts, null will be returned. |  
| [PFAccountManagementGetPlayFabIDsFromFacebookInstantGamesIdsRequest](structs/pfaccountmanagementgetplayfabidsfromfacebookinstantgamesidsrequest.md) | PFAccountManagementGetPlayFabIDsFromFacebookInstantGamesIdsRequest data model. |  
| [PFAccountManagementGetPlayFabIDsFromFacebookInstantGamesIdsResult](structs/pfaccountmanagementgetplayfabidsfromfacebookinstantgamesidsresult.md) | PFAccountManagementGetPlayFabIDsFromFacebookInstantGamesIdsResult data model. For Facebook Instant Game identifiers which have not been linked to PlayFab accounts, null will be returned. |  
| [PFAccountManagementGetPlayFabIDsFromGameCenterIDsRequest](structs/pfaccountmanagementgetplayfabidsfromgamecenteridsrequest.md) | PFAccountManagementGetPlayFabIDsFromGameCenterIDsRequest data model. |  
| [PFAccountManagementGetPlayFabIDsFromGameCenterIDsResult](structs/pfaccountmanagementgetplayfabidsfromgamecenteridsresult.md) | PFAccountManagementGetPlayFabIDsFromGameCenterIDsResult data model. For Game Center identifiers which have not been linked to PlayFab accounts, null will be returned. |  
| [PFAccountManagementGetPlayFabIDsFromGoogleIDsRequest](structs/pfaccountmanagementgetplayfabidsfromgoogleidsrequest.md) | PFAccountManagementGetPlayFabIDsFromGoogleIDsRequest data model. |  
| [PFAccountManagementGetPlayFabIDsFromGoogleIDsResult](structs/pfaccountmanagementgetplayfabidsfromgoogleidsresult.md) | PFAccountManagementGetPlayFabIDsFromGoogleIDsResult data model. For Google identifiers which have not been linked to PlayFab accounts, null will be returned. |  
| [PFAccountManagementGetPlayFabIDsFromGooglePlayGamesPlayerIDsRequest](structs/pfaccountmanagementgetplayfabidsfromgoogleplaygamesplayeridsrequest.md) | PFAccountManagementGetPlayFabIDsFromGooglePlayGamesPlayerIDsRequest data model. |  
| [PFAccountManagementGetPlayFabIDsFromGooglePlayGamesPlayerIDsResult](structs/pfaccountmanagementgetplayfabidsfromgoogleplaygamesplayeridsresult.md) | PFAccountManagementGetPlayFabIDsFromGooglePlayGamesPlayerIDsResult data model. For Google Play Games identifiers which have not been linked to PlayFab accounts, null will be returned. |  
| [PFAccountManagementGetPlayFabIDsFromKongregateIDsRequest](structs/pfaccountmanagementgetplayfabidsfromkongregateidsrequest.md) | PFAccountManagementGetPlayFabIDsFromKongregateIDsRequest data model. |  
| [PFAccountManagementGetPlayFabIDsFromKongregateIDsResult](structs/pfaccountmanagementgetplayfabidsfromkongregateidsresult.md) | PFAccountManagementGetPlayFabIDsFromKongregateIDsResult data model. For Kongregate identifiers which have not been linked to PlayFab accounts, null will be returned. |  
| [PFAccountManagementGetPlayFabIDsFromNintendoServiceAccountIdsRequest](structs/pfaccountmanagementgetplayfabidsfromnintendoserviceaccountidsrequest.md) | PFAccountManagementGetPlayFabIDsFromNintendoServiceAccountIdsRequest data model. |  
| [PFAccountManagementGetPlayFabIDsFromNintendoServiceAccountIdsResult](structs/pfaccountmanagementgetplayfabidsfromnintendoserviceaccountidsresult.md) | PFAccountManagementGetPlayFabIDsFromNintendoServiceAccountIdsResult data model. For Nintendo Service Account identifiers which have not been linked to PlayFab accounts, null will be returned. |  
| [PFAccountManagementGetPlayFabIDsFromNintendoSwitchDeviceIdsRequest](structs/pfaccountmanagementgetplayfabidsfromnintendoswitchdeviceidsrequest.md) | PFAccountManagementGetPlayFabIDsFromNintendoSwitchDeviceIdsRequest data model. |  
| [PFAccountManagementGetPlayFabIDsFromNintendoSwitchDeviceIdsResult](structs/pfaccountmanagementgetplayfabidsfromnintendoswitchdeviceidsresult.md) | PFAccountManagementGetPlayFabIDsFromNintendoSwitchDeviceIdsResult data model. For Nintendo Switch identifiers which have not been linked to PlayFab accounts, null will be returned. |  
| [PFAccountManagementGetPlayFabIDsFromPSNAccountIDsRequest](structs/pfaccountmanagementgetplayfabidsfrompsnaccountidsrequest.md) | PFAccountManagementGetPlayFabIDsFromPSNAccountIDsRequest data model. |  
| [PFAccountManagementGetPlayFabIDsFromPSNAccountIDsResult](structs/pfaccountmanagementgetplayfabidsfrompsnaccountidsresult.md) | PFAccountManagementGetPlayFabIDsFromPSNAccountIDsResult data model. For PlayStation :tm: Network identifiers which have not been linked to PlayFab accounts, null will be returned. |  
| [PFAccountManagementGetPlayFabIDsFromSteamIDsRequest](structs/pfaccountmanagementgetplayfabidsfromsteamidsrequest.md) | PFAccountManagementGetPlayFabIDsFromSteamIDsRequest data model. |  
| [PFAccountManagementGetPlayFabIDsFromSteamIDsResult](structs/pfaccountmanagementgetplayfabidsfromsteamidsresult.md) | PFAccountManagementGetPlayFabIDsFromSteamIDsResult data model. For Steam identifiers which have not been linked to PlayFab accounts, null will be returned. |  
| [PFAccountManagementGetPlayFabIDsFromTwitchIDsRequest](structs/pfaccountmanagementgetplayfabidsfromtwitchidsrequest.md) | PFAccountManagementGetPlayFabIDsFromTwitchIDsRequest data model. |  
| [PFAccountManagementGetPlayFabIDsFromTwitchIDsResult](structs/pfaccountmanagementgetplayfabidsfromtwitchidsresult.md) | PFAccountManagementGetPlayFabIDsFromTwitchIDsResult data model. For Twitch identifiers which have not been linked to PlayFab accounts, null will be returned. |  
| [PFAccountManagementGetPlayFabIDsFromXboxLiveIDsRequest](structs/pfaccountmanagementgetplayfabidsfromxboxliveidsrequest.md) | PFAccountManagementGetPlayFabIDsFromXboxLiveIDsRequest data model. |  
| [PFAccountManagementGetPlayFabIDsFromXboxLiveIDsResult](structs/pfaccountmanagementgetplayfabidsfromxboxliveidsresult.md) | PFAccountManagementGetPlayFabIDsFromXboxLiveIDsResult data model. For XboxLive identifiers which have not been linked to PlayFab accounts, null will be returned. |  
| [PFAccountManagementGetServerCustomIDsFromPlayFabIDsRequest](structs/pfaccountmanagementgetservercustomidsfromplayfabidsrequest.md) | PFAccountManagementGetServerCustomIDsFromPlayFabIDsRequest data model. |  
| [PFAccountManagementGetServerCustomIDsFromPlayFabIDsResult](structs/pfaccountmanagementgetservercustomidsfromplayfabidsresult.md) | PFAccountManagementGetServerCustomIDsFromPlayFabIDsResult data model. For a PlayFab account that isn't associated with a server custom identity, ServerCustomId will be null. |  
| [PFAccountManagementGetTitlePlayersFromProviderIDsResponse](structs/pfaccountmanagementgettitleplayersfromprovideridsresponse.md) | PFAccountManagementGetTitlePlayersFromProviderIDsResponse data model. |  
| [PFAccountManagementGetTitlePlayersFromXboxLiveIDsRequest](structs/pfaccountmanagementgettitleplayersfromxboxliveidsrequest.md) | PFAccountManagementGetTitlePlayersFromXboxLiveIDsRequest data model. Given a collection of Xbox IDs (XUIDs), returns all title player accounts. |  
| [PFAccountManagementGetUserAccountInfoRequest](structs/pfaccountmanagementgetuseraccountinforequest.md) | PFAccountManagementGetUserAccountInfoRequest data model. This API allows for access to details regarding a user in the PlayFab service, usually for purposes of customer support. Note that data returned may be Personally Identifying Information (PII), such as email address, and so care should be taken in how this data is stored and managed. Since this call will always return the relevant information for users who have accessed the title, the recommendation is to not store this data locally. |  
| [PFAccountManagementGetUserAccountInfoResult](structs/pfaccountmanagementgetuseraccountinforesult.md) | PFAccountManagementGetUserAccountInfoResult data model. |  
| [PFAccountManagementGetUserBansRequest](structs/pfaccountmanagementgetuserbansrequest.md) | PFAccountManagementGetUserBansRequest data model. Get all bans for a user, including inactive and expired bans. . |  
| [PFAccountManagementGetUserBansResult](structs/pfaccountmanagementgetuserbansresult.md) | PFAccountManagementGetUserBansResult data model. |  
| [PFAccountManagementGooglePlayFabIdPair](structs/pfaccountmanagementgoogleplayfabidpair.md) | PFAccountManagementGooglePlayFabIdPair data model. |  
| [PFAccountManagementGooglePlayGamesPlayFabIdPair](structs/pfaccountmanagementgoogleplaygamesplayfabidpair.md) | PFAccountManagementGooglePlayGamesPlayFabIdPair data model. |  
| [PFAccountManagementKongregatePlayFabIdPair](structs/pfaccountmanagementkongregateplayfabidpair.md) | PFAccountManagementKongregatePlayFabIdPair data model. |  
| [PFAccountManagementLinkAndroidDeviceIDRequest](structs/pfaccountmanagementlinkandroiddeviceidrequest.md) | PFAccountManagementLinkAndroidDeviceIDRequest data model. |  
| [PFAccountManagementLinkAppleRequest](structs/pfaccountmanagementlinkapplerequest.md) | PFAccountManagementLinkAppleRequest data model. |  
| [PFAccountManagementLinkCustomIDRequest](structs/pfaccountmanagementlinkcustomidrequest.md) | PFAccountManagementLinkCustomIDRequest data model. |  
| [PFAccountManagementLinkFacebookAccountRequest](structs/pfaccountmanagementlinkfacebookaccountrequest.md) | PFAccountManagementLinkFacebookAccountRequest data model. Facebook sign-in is accomplished using the Facebook User Access Token. More information on the Token can be found in the Facebook developer documentation (https://developers.facebook.com/docs/facebook-login/access-tokens/). In Unity, for example, the Token is available as AccessToken in the Facebook SDK ScriptableObject FB. Note that titles should never re-use the same Facebook applications between PlayFab Title IDs, as Facebook provides unique user IDs per application and doing so can result in issues with the Facebook ID for the user in their PlayFab account information. If you must re-use an application in a new PlayFab Title ID, please be sure to first unlink all accounts from Facebook, or delete all users in the first Title ID. |  
| [PFAccountManagementLinkFacebookInstantGamesIdRequest](structs/pfaccountmanagementlinkfacebookinstantgamesidrequest.md) | PFAccountManagementLinkFacebookInstantGamesIdRequest data model. |  
| [PFAccountManagementLinkGameCenterAccountRequest](structs/pfaccountmanagementlinkgamecenteraccountrequest.md) | PFAccountManagementLinkGameCenterAccountRequest data model. |  
| [PFAccountManagementLinkGoogleAccountRequest](structs/pfaccountmanagementlinkgoogleaccountrequest.md) | PFAccountManagementLinkGoogleAccountRequest data model. Google sign-in is accomplished by obtaining a Google OAuth 2.0 credential using the Google sign-in for Android APIs on the device and passing it to this API. |  
| [PFAccountManagementLinkGooglePlayGamesServicesAccountRequest](structs/pfaccountmanagementlinkgoogleplaygamesservicesaccountrequest.md) | PFAccountManagementLinkGooglePlayGamesServicesAccountRequest data model. Google Play Games sign-in is accomplished by obtaining a Google OAuth 2.0 credential using the Google Play Games sign-in for Android APIs on the device and passing it to this API. |  
| [PFAccountManagementLinkIOSDeviceIDRequest](structs/pfaccountmanagementlinkiosdeviceidrequest.md) | PFAccountManagementLinkIOSDeviceIDRequest data model. |  
| [PFAccountManagementLinkKongregateAccountRequest](structs/pfaccountmanagementlinkkongregateaccountrequest.md) | PFAccountManagementLinkKongregateAccountRequest data model. |  
| [PFAccountManagementLinkNintendoServiceAccountSubjectRequest](structs/pfaccountmanagementlinknintendoserviceaccountsubjectrequest.md) | PFAccountManagementLinkNintendoServiceAccountSubjectRequest data model. |  
| [PFAccountManagementLinkOpenIdConnectRequest](structs/pfaccountmanagementlinkopenidconnectrequest.md) | PFAccountManagementLinkOpenIdConnectRequest data model. |  
| [PFAccountManagementLinkServerCustomIdRequest](structs/pfaccountmanagementlinkservercustomidrequest.md) | PFAccountManagementLinkServerCustomIdRequest data model. |  
| [PFAccountManagementLinkSteamAccountRequest](structs/pfaccountmanagementlinksteamaccountrequest.md) | PFAccountManagementLinkSteamAccountRequest data model. Steam authentication is accomplished with the Steam Session Ticket. More information on the Ticket can be found in the Steamworks SDK, here: https://partner.steamgames.com/documentation/auth (requires sign-in). NOTE: For Steam authentication to work, the title must be configured with the Steam Application ID and Publisher Key in the PlayFab Game Manager (under Properties). Information on creating a Publisher Key (referred to as the Secret Key in PlayFab) for your title can be found here: https://partner.steamgames.com/documentation/webapi#publisherkey. |  
| [PFAccountManagementLinkSteamIdRequest](structs/pfaccountmanagementlinksteamidrequest.md) | PFAccountManagementLinkSteamIdRequest data model. |  
| [PFAccountManagementLinkTwitchAccountRequest](structs/pfaccountmanagementlinktwitchaccountrequest.md) | PFAccountManagementLinkTwitchAccountRequest data model. |  
| [PFAccountManagementNintendoServiceAccountPlayFabIdPair](structs/pfaccountmanagementnintendoserviceaccountplayfabidpair.md) | PFAccountManagementNintendoServiceAccountPlayFabIdPair data model. |  
| [PFAccountManagementNintendoSwitchPlayFabIdPair](structs/pfaccountmanagementnintendoswitchplayfabidpair.md) | PFAccountManagementNintendoSwitchPlayFabIdPair data model. |  
| [PFAccountManagementPSNAccountPlayFabIdPair](structs/pfaccountmanagementpsnaccountplayfabidpair.md) | PFAccountManagementPSNAccountPlayFabIdPair data model. |  
| [PFAccountManagementRemoveContactEmailRequest](structs/pfaccountmanagementremovecontactemailrequest.md) | PFAccountManagementRemoveContactEmailRequest data model. This API removes an existing contact email from the player's profile. |  
| [PFAccountManagementReportPlayerClientRequest](structs/pfaccountmanagementreportplayerclientrequest.md) | PFAccountManagementReportPlayerClientRequest data model. |  
| [PFAccountManagementReportPlayerClientResult](structs/pfaccountmanagementreportplayerclientresult.md) | PFAccountManagementReportPlayerClientResult data model. Players are currently limited to five reports per day. Attempts by a single user account to submit reports beyond five will result in Updated being returned as false. |  
| [PFAccountManagementRevokeAllBansForUserRequest](structs/pfaccountmanagementrevokeallbansforuserrequest.md) | PFAccountManagementRevokeAllBansForUserRequest data model. Setting the active state of all non-expired bans for a user to Inactive. Expired bans with an Active state will be ignored, however. Returns information about applied updates only. |  
| [PFAccountManagementRevokeAllBansForUserResult](structs/pfaccountmanagementrevokeallbansforuserresult.md) | PFAccountManagementRevokeAllBansForUserResult data model. |  
| [PFAccountManagementRevokeBansRequest](structs/pfaccountmanagementrevokebansrequest.md) | PFAccountManagementRevokeBansRequest data model. Setting the active state of all bans requested to Inactive regardless of whether that ban has already expired. BanIds that do not exist will be skipped. Returns information about applied updates only. . |  
| [PFAccountManagementRevokeBansResult](structs/pfaccountmanagementrevokebansresult.md) | PFAccountManagementRevokeBansResult data model. |  
| [PFAccountManagementSendAccountRecoveryEmailRequest](structs/pfaccountmanagementsendaccountrecoveryemailrequest.md) | PFAccountManagementSendAccountRecoveryEmailRequest data model. If the account in question is a "temporary" account (for example, one that was created via a call to LoginFromIOSDeviceID), thisfunction will have no effect. Only PlayFab accounts which have valid email addresses will be able to receive a password reset email using this API. |  
| [PFAccountManagementSendCustomAccountRecoveryEmailRequest](structs/pfaccountmanagementsendcustomaccountrecoveryemailrequest.md) | PFAccountManagementSendCustomAccountRecoveryEmailRequest data model. PlayFab accounts which have valid email address or username will be able to receive a password reset email using this API.The email sent must be an account recovery email template. The username or email can be passed in to send the email. |  
| [PFAccountManagementSendEmailFromTemplateRequest](structs/pfaccountmanagementsendemailfromtemplaterequest.md) | PFAccountManagementSendEmailFromTemplateRequest data model. Sends an email for only players that have contact emails associated with them. Takes in an email template ID specifyingthe email template to send. |  
| [PFAccountManagementServerCustomIDPlayFabIDPair](structs/pfaccountmanagementservercustomidplayfabidpair.md) | PFAccountManagementServerCustomIDPlayFabIDPair data model. |  
| [PFAccountManagementServerLinkNintendoServiceAccountRequest](structs/pfaccountmanagementserverlinknintendoserviceaccountrequest.md) | PFAccountManagementServerLinkNintendoServiceAccountRequest data model. |  
| [PFAccountManagementServerLinkNintendoSwitchDeviceIdRequest](structs/pfaccountmanagementserverlinknintendoswitchdeviceidrequest.md) | PFAccountManagementServerLinkNintendoSwitchDeviceIdRequest data model. |  
| [PFAccountManagementServerLinkPSNAccountRequest](structs/pfaccountmanagementserverlinkpsnaccountrequest.md) | PFAccountManagementServerLinkPSNAccountRequest data model. |  
| [PFAccountManagementServerLinkXboxAccountRequest](structs/pfaccountmanagementserverlinkxboxaccountrequest.md) | PFAccountManagementServerLinkXboxAccountRequest data model. |  
| [PFAccountManagementServerUnlinkNintendoServiceAccountRequest](structs/pfaccountmanagementserverunlinknintendoserviceaccountrequest.md) | PFAccountManagementServerUnlinkNintendoServiceAccountRequest data model. |  
| [PFAccountManagementServerUnlinkNintendoSwitchDeviceIdRequest](structs/pfaccountmanagementserverunlinknintendoswitchdeviceidrequest.md) | PFAccountManagementServerUnlinkNintendoSwitchDeviceIdRequest data model. |  
| [PFAccountManagementServerUnlinkPSNAccountRequest](structs/pfaccountmanagementserverunlinkpsnaccountrequest.md) | PFAccountManagementServerUnlinkPSNAccountRequest data model. |  
| [PFAccountManagementServerUnlinkXboxAccountRequest](structs/pfaccountmanagementserverunlinkxboxaccountrequest.md) | PFAccountManagementServerUnlinkXboxAccountRequest data model. |  
| [PFAccountManagementServerUpdateAvatarUrlRequest](structs/pfaccountmanagementserverupdateavatarurlrequest.md) | PFAccountManagementServerUpdateAvatarUrlRequest data model. |  
| [PFAccountManagementSteamPlayFabIdPair](structs/pfaccountmanagementsteamplayfabidpair.md) | PFAccountManagementSteamPlayFabIdPair data model. |  
| [PFAccountManagementTwitchPlayFabIdPair](structs/pfaccountmanagementtwitchplayfabidpair.md) | PFAccountManagementTwitchPlayFabIdPair data model. |  
| [PFAccountManagementUnlinkAndroidDeviceIDRequest](structs/pfaccountmanagementunlinkandroiddeviceidrequest.md) | PFAccountManagementUnlinkAndroidDeviceIDRequest data model. |  
| [PFAccountManagementUnlinkAppleRequest](structs/pfaccountmanagementunlinkapplerequest.md) | PFAccountManagementUnlinkAppleRequest data model. |  
| [PFAccountManagementUnlinkCustomIDRequest](structs/pfaccountmanagementunlinkcustomidrequest.md) | PFAccountManagementUnlinkCustomIDRequest data model. |  
| [PFAccountManagementUnlinkFacebookAccountRequest](structs/pfaccountmanagementunlinkfacebookaccountrequest.md) | PFAccountManagementUnlinkFacebookAccountRequest data model. |  
| [PFAccountManagementUnlinkFacebookInstantGamesIdRequest](structs/pfaccountmanagementunlinkfacebookinstantgamesidrequest.md) | PFAccountManagementUnlinkFacebookInstantGamesIdRequest data model. |  
| [PFAccountManagementUnlinkGameCenterAccountRequest](structs/pfaccountmanagementunlinkgamecenteraccountrequest.md) | PFAccountManagementUnlinkGameCenterAccountRequest data model. |  
| [PFAccountManagementUnlinkGoogleAccountRequest](structs/pfaccountmanagementunlinkgoogleaccountrequest.md) | PFAccountManagementUnlinkGoogleAccountRequest data model. |  
| [PFAccountManagementUnlinkGooglePlayGamesServicesAccountRequest](structs/pfaccountmanagementunlinkgoogleplaygamesservicesaccountrequest.md) | PFAccountManagementUnlinkGooglePlayGamesServicesAccountRequest data model. |  
| [PFAccountManagementUnlinkIOSDeviceIDRequest](structs/pfaccountmanagementunlinkiosdeviceidrequest.md) | PFAccountManagementUnlinkIOSDeviceIDRequest data model. |  
| [PFAccountManagementUnlinkKongregateAccountRequest](structs/pfaccountmanagementunlinkkongregateaccountrequest.md) | PFAccountManagementUnlinkKongregateAccountRequest data model. |  
| [PFAccountManagementUnlinkOpenIdConnectRequest](structs/pfaccountmanagementunlinkopenidconnectrequest.md) | PFAccountManagementUnlinkOpenIdConnectRequest data model. |  
| [PFAccountManagementUnlinkServerCustomIdRequest](structs/pfaccountmanagementunlinkservercustomidrequest.md) | PFAccountManagementUnlinkServerCustomIdRequest data model. |  
| [PFAccountManagementUnlinkSteamAccountRequest](structs/pfaccountmanagementunlinksteamaccountrequest.md) | PFAccountManagementUnlinkSteamAccountRequest data model. |  
| [PFAccountManagementUnlinkSteamIdRequest](structs/pfaccountmanagementunlinksteamidrequest.md) | PFAccountManagementUnlinkSteamIdRequest data model. |  
| [PFAccountManagementUnlinkTwitchAccountRequest](structs/pfaccountmanagementunlinktwitchaccountrequest.md) | PFAccountManagementUnlinkTwitchAccountRequest data model. |  
| [PFAccountManagementUpdateBanRequest](structs/pfaccountmanagementupdatebanrequest.md) | PFAccountManagementUpdateBanRequest data model. Represents a single update ban request. |  
| [PFAccountManagementUpdateBansRequest](structs/pfaccountmanagementupdatebansrequest.md) | PFAccountManagementUpdateBansRequest data model. For each ban, only updates the values that are set. Leave any value to null for no change. If a ban could not be found, the rest are still applied. Returns information about applied updates only. |  
| [PFAccountManagementUpdateBansResult](structs/pfaccountmanagementupdatebansresult.md) | PFAccountManagementUpdateBansResult data model. |  
| [PFAccountManagementUpdateUserTitleDisplayNameRequest](structs/pfaccountmanagementupdateusertitledisplaynamerequest.md) | PFAccountManagementUpdateUserTitleDisplayNameRequest data model. In addition to the PlayFab username, titles can make use of a DisplayName which is also a unique identifier, but specific to the title. This allows for unique names which more closely match the theme or genre of a title, for example. |  
| [PFAccountManagementUpdateUserTitleDisplayNameResult](structs/pfaccountmanagementupdateusertitledisplaynameresult.md) | PFAccountManagementUpdateUserTitleDisplayNameResult data model. |  
| [PFAccountManagementXboxLiveAccountPlayFabIdPair](structs/pfaccountmanagementxboxliveaccountplayfabidpair.md) | PFAccountManagementXboxLiveAccountPlayFabIdPair data model. |  