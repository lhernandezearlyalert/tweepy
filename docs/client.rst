.. _client_reference:

.. currentmodule:: tweepy

***************************************************
:class:`tweepy.Client` --- Twitter API v2 Reference
***************************************************

.. autoclass:: Client

.. table::
    :align: center

    +--------------------------------------------------------------+----------------------------------------+
    | Twitter API v2 Endpoint                                      | :class:`Client` Method                 |
    +==============================================================+========================================+
    | .. centered:: :ref:`Tweets`                                                                           |
    +-------------------------------------------------------------------------------------------------------+
    | .. centered:: |Hide replies|_                                                                         |
    +--------------------------------------------------------------+----------------------------------------+
    | `PUT /2/tweets/:id/hidden`_                                  | :meth:`Client.hide_reply`              |
    +--------------------------------------------------------------+----------------------------------------+
    | `PUT /2/tweets/:id/hidden`_                                  | :meth:`Client.unhide_reply`            |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: |Likes|_                                                                                |
    +--------------------------------------------------------------+----------------------------------------+
    | `DELETE /2/users/:id/likes/:tweet_id`_                       | :meth:`Client.unlike`                  |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/tweets/:id/liking_users`_                            | :meth:`Client.get_liking_users`        |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/users/:id/liked_tweets`_                             | :meth:`Client.get_liked_tweets`        |
    +--------------------------------------------------------------+----------------------------------------+
    | `POST /2/users/:id/likes`_                                   | :meth:`Client.like`                    |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: |Manage Tweets|_                                                                        |
    +--------------------------------------------------------------+----------------------------------------+
    | `DELETE /2/tweets/:id`_                                      | :meth:`Client.delete_tweet`            |
    +--------------------------------------------------------------+----------------------------------------+
    | `POST /2/tweets`_                                            | :meth:`Client.create_tweet`            |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: |Retweets|_                                                                             |
    +--------------------------------------------------------------+----------------------------------------+
    | `DELETE /2/users/:id/retweets/:source_tweet_id`_             | :meth:`Client.unretweet`               |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/tweets/:id/retweeted_by`_                            | :meth:`Client.get_retweeters`          |
    +--------------------------------------------------------------+----------------------------------------+
    | `POST /2/users/:id/retweets`_                                | :meth:`Client.retweet`                 |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: |Search Tweets|_                                                                        |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/tweets/search/all`_                                  | :meth:`Client.search_all_tweets`       |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/tweets/search/recent`_                               | :meth:`Client.search_recent_tweets`    |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: |Timelines|_                                                                            |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/users/:id/mentions`_                                 | :meth:`Client.get_users_mentions`      |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/users/:id/tweets`_                                   | :meth:`Client.get_users_tweets`        |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: |Tweet counts|_                                                                         |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/tweets/counts/all`_                                  | :meth:`Client.get_all_tweets_count`    |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/tweets/counts/recent`_                               | :meth:`Client.get_recent_tweets_count` |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: |Tweet lookup|_                                                                         |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/tweets/:id`_                                         | :meth:`Client.get_tweet`               |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/tweets`_                                             | :meth:`Client.get_tweets`              |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: :ref:`Users`                                                                            |
    +-------------------------------------------------------------------------------------------------------+
    | .. centered:: |Blocks|_                                                                               |
    +--------------------------------------------------------------+----------------------------------------+
    | `DELETE /2/users/:source_user_id/blocking/:target_user_id`_  | :meth:`Client.unblock`                 |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/users/:id/blocking`_                                 | :meth:`Client.get_blocked`             |
    +--------------------------------------------------------------+----------------------------------------+
    | `POST /2/users/:id/blocking`_                                | :meth:`Client.block`                   |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: |Follows|_                                                                              |
    +--------------------------------------------------------------+----------------------------------------+
    | `DELETE /2/users/:source_user_id/following/:target_user_id`_ | :meth:`Client.unfollow_user`           |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/users/:id/followers`_                                | :meth:`Client.get_users_followers`     |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/users/:id/following`_                                | :meth:`Client.get_users_following`     |
    +--------------------------------------------------------------+----------------------------------------+
    | `POST /2/users/:id/following`_                               | :meth:`Client.follow_user`             |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: |Mutes|_                                                                                |
    +--------------------------------------------------------------+----------------------------------------+
    | `DELETE /2/users/:source_user_id/muting/:target_user_id`_    | :meth:`Client.unmute`                  |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/users/:id/muting`_                                   | :meth:`Client.get_muted`               |
    +--------------------------------------------------------------+----------------------------------------+
    | `POST /2/users/:id/muting`_                                  | :meth:`Client.mute`                    |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: |User lookup|_                                                                          |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/users/:id`_                                          | :meth:`Client.get_user`                |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/users/by/username/:username`_                        | :meth:`Client.get_user`                |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/users`_                                              | :meth:`Client.get_users`               |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/users/by`_                                           | :meth:`Client.get_users`               |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/users/me`_                                           | :meth:`Client.get_me`                  |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: :ref:`Spaces`                                                                           |
    +-------------------------------------------------------------------------------------------------------+
    | .. centered:: |Search Spaces|_                                                                        |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/spaces/search`_                                      | :meth:`Client.search_spaces`           |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: |Spaces lookup|_                                                                        |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/spaces`_                                             | :meth:`Client.get_spaces`              |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/spaces/:id`_                                         | :meth:`Client.get_space`               |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/spaces/:id/buyers`_                                  | :meth:`Client.get_space_buyers`        |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/spaces/by/creator_ids`_                              | :meth:`Client.get_spaces`              |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: :ref:`Lists`                                                                            |
    +-------------------------------------------------------------------------------------------------------+
    | .. centered:: |List Tweets lookup|_                                                                   |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/lists/:id/tweets`_                                   | :meth:`Client.get_list_tweets`         |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: |List follows|_                                                                         |
    +--------------------------------------------------------------+----------------------------------------+
    | `DELETE /2/users/:id/followed_lists/:list_id`_               | :meth:`Client.unfollow_list`           |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/lists/:id/followers`_                                | :meth:`Client.get_list_followers`      |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/users/:id/followed_lists`_                           | :meth:`Client.get_followed_lists`      |
    +--------------------------------------------------------------+----------------------------------------+
    | `POST /2/users/:id/followed_lists`_                          | :meth:`Client.follow_list`             |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: |List lookup|_                                                                          |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/lists/:id`_                                          | :meth:`Client.get_list`                |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/users/:id/owned_lists`_                              | :meth:`Client.get_owned_lists`         |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: |List members|_                                                                         |
    +--------------------------------------------------------------+----------------------------------------+
    | `DELETE /2/lists/:id/members/:user_id`_                      | :meth:`Client.remove_list_member`      |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/lists/:id/members`_                                  | :meth:`Client.get_list_members`        |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/users/:id/list_memberships`_                         | :meth:`Client.get_list_memberships`    |
    +--------------------------------------------------------------+----------------------------------------+
    | `POST /2/lists/:id/members`_                                 | :meth:`Client.add_list_member`         |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: |Manage Lists|_                                                                         |
    +--------------------------------------------------------------+----------------------------------------+
    | `DELETE /2/lists/:id`_                                       | :meth:`Client.delete_list`             |
    +--------------------------------------------------------------+----------------------------------------+
    | `PUT /2/lists/:id`_                                          | :meth:`Client.update_list`             |
    +--------------------------------------------------------------+----------------------------------------+
    | `POST /2/lists`_                                             | :meth:`Client.create_list`             |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: |Pinned Lists|_                                                                         |
    +--------------------------------------------------------------+----------------------------------------+
    | `DELETE /2/users/:id/pinned_lists/:list_id`_                 | :meth:`Client.unpin_list`              |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/users/:id/pinned_lists`_                             | :meth:`Client.get_pinned_lists`        |
    +--------------------------------------------------------------+----------------------------------------+
    | `POST /2/users/:id/pinned_lists`_                            | :meth:`Client.pin_list`                |
    +--------------------------------------------------------------+----------------------------------------+
    | .. centered:: :ref:`Compliance`                                                                       |
    +-------------------------------------------------------------------------------------------------------+
    | .. centered:: |Batch Compliance|_                                                                     |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/compliance/jobs`_                                    | :meth:`Client.get_compliance_jobs`     |
    +--------------------------------------------------------------+----------------------------------------+
    | `GET /2/compliance/jobs/:id`_                                | :meth:`Client.get_compliance_job`      |
    +--------------------------------------------------------------+----------------------------------------+
    | `POST /2/compliance/jobs`_                                   | :meth:`Client.create_compliance_job`   |
    +--------------------------------------------------------------+----------------------------------------+

.. |Hide replies| replace:: *Hide replies*
.. _PUT /2/tweets/:id/hidden: https://developer.twitter.com/en/docs/twitter-api/tweets/hide-replies/api-reference/put-tweets-id-hidden
.. |Likes| replace:: *Likes*
.. _DELETE /2/users/:id/likes/:tweet_id: https://developer.twitter.com/en/docs/twitter-api/tweets/likes/api-reference/delete-users-id-likes-tweet_id
.. _GET /2/tweets/:id/liking_users: https://developer.twitter.com/en/docs/twitter-api/tweets/likes/api-reference/get-tweets-id-liking_users
.. _GET /2/users/:id/liked_tweets: https://developer.twitter.com/en/docs/twitter-api/tweets/likes/api-reference/get-users-id-liked_tweets
.. _POST /2/users/:id/likes: https://developer.twitter.com/en/docs/twitter-api/tweets/likes/api-reference/post-users-id-likes
.. |Manage Tweets| replace:: *Manage Tweets*
.. _DELETE /2/tweets/:id: https://developer.twitter.com/en/docs/twitter-api/tweets/manage-tweets/api-reference/delete-tweets-id
.. _POST /2/tweets: https://developer.twitter.com/en/docs/twitter-api/tweets/manage-tweets/api-reference/post-tweets
.. |Retweets| replace:: *Retweets*
.. _DELETE /2/users/:id/retweets/:source_tweet_id: https://developer.twitter.com/en/docs/twitter-api/tweets/retweets/api-reference/delete-users-id-retweets-tweet_id
.. _GET /2/tweets/:id/retweeted_by: https://developer.twitter.com/en/docs/twitter-api/tweets/retweets/api-reference/get-tweets-id-retweeted_by
.. _POST /2/users/:id/retweets: https://developer.twitter.com/en/docs/twitter-api/tweets/retweets/api-reference/post-users-id-retweets
.. |Search Tweets| replace:: *Search Tweets*
.. _GET /2/tweets/search/all: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-all
.. _GET /2/tweets/search/recent: https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-recent
.. |Timelines| replace:: *Timelines*
.. _GET /2/users/:id/mentions: https://developer.twitter.com/en/docs/twitter-api/tweets/timelines/api-reference/get-users-id-mentions
.. _GET /2/users/:id/tweets: https://developer.twitter.com/en/docs/twitter-api/tweets/timelines/api-reference/get-users-id-tweets
.. |Tweet counts| replace:: *Tweet counts*
.. _GET /2/tweets/counts/all: https://developer.twitter.com/en/docs/twitter-api/tweets/counts/api-reference/get-tweets-counts-all
.. _GET /2/tweets/counts/recent: https://developer.twitter.com/en/docs/twitter-api/tweets/counts/api-reference/get-tweets-counts-recent
.. |Tweet lookup| replace:: *Tweet lookup*
.. _GET /2/tweets/:id: https://developer.twitter.com/en/docs/twitter-api/tweets/lookup/api-reference/get-tweets-id
.. _GET /2/tweets: https://developer.twitter.com/en/docs/twitter-api/tweets/lookup/api-reference/get-tweets
.. |Blocks| replace:: *Blocks*
.. _DELETE /2/users/:source_user_id/blocking/:target_user_id: https://developer.twitter.com/en/docs/twitter-api/users/blocks/api-reference/delete-users-user_id-blocking
.. _GET /2/users/:id/blocking: https://developer.twitter.com/en/docs/twitter-api/users/blocks/api-reference/get-users-blocking
.. _POST /2/users/:id/blocking: https://developer.twitter.com/en/docs/twitter-api/users/blocks/api-reference/post-users-user_id-blocking
.. |Follows| replace:: *Follows*
.. _DELETE /2/users/:source_user_id/following/:target_user_id: https://developer.twitter.com/en/docs/twitter-api/users/follows/api-reference/delete-users-source_id-following
.. _GET /2/users/:id/followers: https://developer.twitter.com/en/docs/twitter-api/users/follows/api-reference/get-users-id-followers
.. _GET /2/users/:id/following: https://developer.twitter.com/en/docs/twitter-api/users/follows/api-reference/get-users-id-following
.. _POST /2/users/:id/following: https://developer.twitter.com/en/docs/twitter-api/users/follows/api-reference/post-users-source_user_id-following
.. |Mutes| replace:: *Mutes*
.. _DELETE /2/users/:source_user_id/muting/:target_user_id: https://developer.twitter.com/en/docs/twitter-api/users/mutes/api-reference/delete-users-user_id-muting
.. _GET /2/users/:id/muting: https://developer.twitter.com/en/docs/twitter-api/users/mutes/api-reference/get-users-muting
.. _POST /2/users/:id/muting: https://developer.twitter.com/en/docs/twitter-api/users/mutes/api-reference/post-users-user_id-muting
.. |User lookup| replace:: *User lookup*
.. _GET /2/users/:id: https://developer.twitter.com/en/docs/twitter-api/users/lookup/api-reference/get-users-id
.. _GET /2/users/by/username/:username: https://developer.twitter.com/en/docs/twitter-api/users/lookup/api-reference/get-users-by-username-username
.. _GET /2/users: https://developer.twitter.com/en/docs/twitter-api/users/lookup/api-reference/get-users
.. _GET /2/users/by: https://developer.twitter.com/en/docs/twitter-api/users/lookup/api-reference/get-users-by
.. _GET /2/users/me: https://developer.twitter.com/en/docs/twitter-api/users/lookup/api-reference/get-users-me
.. |Search Spaces| replace:: *Search Spaces*
.. _GET /2/spaces/search: https://developer.twitter.com/en/docs/twitter-api/spaces/search/api-reference/get-spaces-search
.. |Spaces lookup| replace:: *Spaces lookup*
.. _GET /2/spaces: https://developer.twitter.com/en/docs/twitter-api/spaces/lookup/api-reference/get-spaces
.. _GET /2/spaces/:id: https://developer.twitter.com/en/docs/twitter-api/spaces/lookup/api-reference/get-spaces-id
.. _GET /2/spaces/:id/buyers: https://developer.twitter.com/en/docs/twitter-api/spaces/lookup/api-reference/get-spaces-id-buyers
.. _GET /2/spaces/by/creator_ids: https://developer.twitter.com/en/docs/twitter-api/spaces/lookup/api-reference/get-spaces-by-creator-ids
.. |List Tweets lookup| replace:: *List Tweets lookup*
.. _GET /2/lists/:id/tweets: https://developer.twitter.com/en/docs/twitter-api/lists/list-tweets/api-reference/get-lists-id-tweets
.. |List follows| replace:: *List follows*
.. _DELETE /2/users/:id/followed_lists/:list_id: https://developer.twitter.com/en/docs/twitter-api/lists/list-follows/api-reference/delete-users-id-followed-lists-list_id
.. _GET /2/lists/:id/followers: https://developer.twitter.com/en/docs/twitter-api/lists/list-follows/api-reference/get-lists-id-followers
.. _GET /2/users/:id/followed_lists: https://developer.twitter.com/en/docs/twitter-api/lists/list-follows/api-reference/get-users-id-followed_lists
.. _POST /2/users/:id/followed_lists: https://developer.twitter.com/en/docs/twitter-api/lists/list-follows/api-reference/post-users-id-followed-lists
.. |List lookup| replace:: *List lookup*
.. _GET /2/lists/:id: https://developer.twitter.com/en/docs/twitter-api/lists/list-lookup/api-reference/get-lists-id
.. _GET /2/users/:id/owned_lists: https://developer.twitter.com/en/docs/twitter-api/lists/list-lookup/api-reference/get-users-id-owned_lists
.. |List members| replace:: *List members*
.. _DELETE /2/lists/:id/members/:user_id: https://developer.twitter.com/en/docs/twitter-api/lists/list-members/api-reference/delete-lists-id-members-user_id
.. _GET /2/lists/:id/members: https://developer.twitter.com/en/docs/twitter-api/lists/list-members/api-reference/get-lists-id-members
.. _GET /2/users/:id/list_memberships: https://developer.twitter.com/en/docs/twitter-api/lists/list-members/api-reference/get-users-id-list_memberships
.. _POST /2/lists/:id/members: https://developer.twitter.com/en/docs/twitter-api/lists/list-members/api-reference/post-lists-id-members
.. |Manage Lists| replace:: *Manage Lists*
.. _DELETE /2/lists/:id: https://developer.twitter.com/en/docs/twitter-api/lists/manage-lists/api-reference/delete-lists-id
.. _PUT /2/lists/:id: https://developer.twitter.com/en/docs/twitter-api/lists/manage-lists/api-reference/put-lists-id
.. _POST /2/lists: https://developer.twitter.com/en/docs/twitter-api/lists/manage-lists/api-reference/post-lists
.. |Pinned Lists| replace:: *Pinned Lists*
.. _DELETE /2/users/:id/pinned_lists/:list_id: https://developer.twitter.com/en/docs/twitter-api/lists/pinned-lists/api-reference/delete-users-id-pinned-lists-list_id
.. _GET /2/users/:id/pinned_lists: https://developer.twitter.com/en/docs/twitter-api/lists/pinned-lists/api-reference/get-users-id-pinned_lists
.. _POST /2/users/:id/pinned_lists: https://developer.twitter.com/en/docs/twitter-api/lists/pinned-lists/api-reference/post-users-id-pinned-lists
.. |Batch Compliance| replace:: *Batch Compliance*
.. _GET /2/compliance/jobs: https://developer.twitter.com/en/docs/twitter-api/compliance/batch-compliance/api-reference/get-compliance-jobs
.. _GET /2/compliance/jobs/:id: https://developer.twitter.com/en/docs/twitter-api/compliance/batch-compliance/api-reference/get-compliance-jobs-id
.. _POST /2/compliance/jobs: https://developer.twitter.com/en/docs/twitter-api/compliance/batch-compliance/api-reference/post-compliance-jobs

Tweets
======

Hide replies
------------

.. automethod:: Client.hide_reply

.. automethod:: Client.unhide_reply

Likes
-----

.. automethod:: Client.unlike

.. automethod:: Client.get_liking_users

.. automethod:: Client.get_liked_tweets

.. automethod:: Client.like

Manage Tweets
-------------

.. automethod:: Client.delete_tweet

.. automethod:: Client.create_tweet

Retweets
--------

.. automethod:: Client.unretweet

.. automethod:: Client.get_retweeters

.. automethod:: Client.retweet

Search Tweets
-------------

.. automethod:: Client.search_all_tweets

.. automethod:: Client.search_recent_tweets

Timelines
---------

.. automethod:: Client.get_users_mentions

.. automethod:: Client.get_users_tweets

Tweet counts
------------

.. automethod:: Client.get_all_tweets_count

.. automethod:: Client.get_recent_tweets_count

Tweet lookup
------------

.. automethod:: Client.get_tweet

.. automethod:: Client.get_tweets

Users
=====

Blocks
------

.. automethod:: Client.unblock

.. automethod:: Client.get_blocked

.. automethod:: Client.block

Follows
-------

.. automethod:: Client.unfollow_user

.. automethod:: Client.unfollow

.. automethod:: Client.get_users_followers

.. automethod:: Client.get_users_following

.. automethod:: Client.follow_user

.. automethod:: Client.follow

Mutes
-----

.. automethod:: Client.unmute

.. automethod:: Client.get_muted

.. automethod:: Client.mute

User lookup
-----------

.. automethod:: Client.get_user

.. automethod:: Client.get_users

.. automethod:: Client.get_me

Spaces
======

Search Spaces
-------------

.. automethod:: Client.search_spaces

Spaces lookup
-------------

.. automethod:: Client.get_spaces

.. automethod:: Client.get_space

.. automethod:: Client.get_space_buyers

Lists
=====

List Tweets lookup
------------------

.. automethod:: Client.get_list_tweets

List follows
------------

.. automethod:: Client.unfollow_list

.. automethod:: Client.get_list_followers

.. automethod:: Client.get_followed_lists

.. automethod:: Client.follow_list

List lookup
-----------

.. automethod:: Client.get_list

.. automethod:: Client.get_owned_lists

List members
------------

.. automethod:: Client.remove_list_member

.. automethod:: Client.get_list_members

.. automethod:: Client.get_list_memberships

.. automethod:: Client.add_list_member

Manage Lists
------------

.. automethod:: Client.delete_list

.. automethod:: Client.update_list

.. automethod:: Client.create_list

Pinned Lists
------------

.. automethod:: Client.unpin_list

.. automethod:: Client.get_pinned_lists

.. automethod:: Client.pin_list

Compliance
==========

Batch compliance
----------------

.. automethod:: Client.get_compliance_jobs

.. automethod:: Client.get_compliance_job

.. automethod:: Client.create_compliance_job

Expansions and Fields Parameters
================================

.. _expansions_parameter:

``expansions``
--------------
`Expansions`_ enable you to request additional data objects that relate to the
originally returned List, Space, Tweets, or users. Submit a list of desired
expansions in a comma-separated list without spaces. The ID that represents the
expanded data object will be included directly in the List, Space, Tweet, or
user data object, but the expanded object metadata will be returned within the
``includes`` response object, and will also include the ID so that you can
match this data object to the original Space, Tweet, or user object.

At this time, the only expansion available to endpoints that primarily return
List objects is ``expansions=owner_id``. You will find the expanded user data
object living in the ``includes`` response object.

For methods that return Spaces, the following data objects can be expanded
using this parameter:

* The Spaces creator's user object
* The user objects of any Space co-host
* Any mentioned users’ object
* Any speaker's user object

For methods that return Tweets, the following data objects can be expanded
using this parameter:

* The Tweet author's user object
* The user object of the Tweet’s author that the
  original Tweet is responding to
* Any mentioned users’ object
* Any referenced Tweets’ author’s user object
* Attached media’s object
* Attached poll’s object
* Attached place’s object
* Any referenced Tweets’ object

At this time, the only expansion available to endpoints that primarily return
user objects is ``expansions=pinned_tweet_id``. You will find the expanded
Tweet data object living in the ``includes`` response object.

.. _list_fields_parameter:

``list_fields``
---------------
This `fields`_ parameter enables you to select which specific `List fields`_
will deliver with each returned List objects. Specify the desired fields in a
comma-separated list without spaces between commas and fields. These specified
List fields will display directly in the List data objects.

.. _media_fields_parameter:

``media_fields``
----------------
This `fields`_ parameter enables you to select which specific `media fields`_
will deliver in each returned Tweet. Specify the desired fields in a
comma-separated list without spaces between commas and fields. The Tweet will
only return media fields if the Tweet contains media and if you've also
included the ``expansions=attachments.media_keys`` query parameter in your
request. While the media ID will be located in the Tweet object, you will find
this ID and all additional media fields in the ``includes`` data object.

.. _place_fields_parameter:

``place_fields``
----------------
This `fields`_ parameter enables you to select which specific `place fields`_
will deliver in each returned Tweet. Specify the desired fields in a
comma-separated list without spaces between commas and fields. The Tweet will
only return place fields if the Tweet contains a place and if you've also
included the ``expansions=geo.place_id`` query parameter in your request. While
the place ID will be located in the Tweet object, you will find this ID and all
additional place fields in the ``includes`` data object.

.. _poll_fields_parameter:

``poll_fields``
---------------

This `fields`_ parameter enables you to select which specific `poll fields`_
will deliver in each returned Tweet. Specify the desired fields in a
comma-separated list without spaces between commas and fields. The Tweet will
only return poll fields if the Tweet contains a poll and if you've also
included the ``expansions=attachments.poll_ids`` query parameter in your
request. While the poll ID will be located in the Tweet object, you will find
this ID and all additional poll fields in the ``includes`` data object.

.. _space_fields_parameter:

``space_fields``
----------------

This `fields`_ parameter enables you to select which specific `Space fields`_
will deliver in each returned Space. Specify the desired fields in a
comma-separated list.

.. _tweet_fields_parameter:

``tweet_fields``
----------------

For methods that return Tweets, this `fields`_ parameter enables you to select
which specific `Tweet fields`_ will deliver in each returned Tweet object.
Specify the desired fields in a comma-separated list without spaces between
commas and fields. You can also pass the ``expansions=referenced_tweets.id``
expansion to return the specified fields for both the original Tweet and any
included referenced Tweets. The requested Tweet fields will display in both the
original Tweet data object, as well as in the referenced Tweet expanded data
object that will be located in the ``includes`` data object.

For methods that return users, this `fields`_ parameter enables you to select
which specific `Tweet fields`_ will deliver in each returned pinned Tweet.
Specify the desired fields in a comma-separated list without spaces between
commas and fields. The Tweet fields will only return if the user has a pinned
Tweet and if you've also included the ``expansions=pinned_tweet_id`` query
parameter in your request. While the referenced Tweet ID will be located in the
original Tweet object, you will find this ID and all additional Tweet fields in
the ``includes`` data object.

.. _user_fields_parameter:

``user_fields``
---------------

For methods that return Spaces or Tweets, this `fields`_ parameter enables you
to select which specific `user fields`_ will deliver in each returned Space or
Tweet. Specify the desired fields in a comma-separated list without spaces
between commas and fields. While the user ID will be located in the original
Tweet object, you will find this ID and all additional user fields in the
``includes`` data object.

You must also pass one of the user expansions to return the desired user
fields:

* ``expansions=author_id``
* ``expansions=entities.mentions.username``
* ``expansions=in_reply_to_user_id``
* ``expansions=referenced_tweets.id.author_id``

For methods that return users, this `fields`_ parameter enables you to select
which specific `user fields`_ will deliver with each returned users objects.
Specify the desired fields in a comma-separated list without spaces between
commas and fields. These specified user fields will display directly in the
user data objects.

.. _Expansions: https://developer.twitter.com/en/docs/twitter-api/expansions
.. _fields: https://developer.twitter.com/en/docs/twitter-api/fields
.. _list fields: https://developer.twitter.com/en/docs/twitter-api/data-dictionary/object-model/lists
.. _media fields: https://developer.twitter.com/en/docs/twitter-api/data-dictionary/object-model/media
.. _place fields: https://developer.twitter.com/en/docs/twitter-api/data-dictionary/object-model/place
.. _poll fields: https://developer.twitter.com/en/docs/twitter-api/data-dictionary/object-model/poll
.. _Space fields: https://developer.twitter.com/en/docs/twitter-api/data-dictionary/object-model/space
.. _Tweet fields: https://developer.twitter.com/en/docs/twitter-api/data-dictionary/object-model/tweet
.. _user fields: https://developer.twitter.com/en/docs/twitter-api/data-dictionary/object-model/user

``Response``
============
.. autoclass:: Response

   The :obj:`Response` returned by :class:`Client` methods is a
   :class:`collections.namedtuple`, with ``data``, ``includes``, ``errors``,
   and ``meta`` fields, corresponding with the fields in responses from
   Twitter's API.

   .. versionadded:: 4.0
