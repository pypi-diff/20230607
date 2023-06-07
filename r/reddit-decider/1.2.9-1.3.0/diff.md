# Comparing `tmp/reddit_decider-1.2.9.tar.gz` & `tmp/reddit_decider-1.3.0.tar.gz`

## Comparing `reddit_decider-1.2.9.tar` & `reddit_decider-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
--rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 reddit_decider-1.2.9/local_dependencies/decider/Cargo.toml
--rw-r--r--   0        0        0       19 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/local_dependencies/decider/.gitignore
--rw-r--r--   0        0        0      710 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/local_dependencies/decider/README.md
--rw-r--r--   0        0        0     6148 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/local_dependencies/decider/benches/decider.rs
--rw-r--r--   0        0        0    46902 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/local_dependencies/decider/src/events.rs
--rw-r--r--   0        0        0    80028 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/local_dependencies/decider/src/lib.rs
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 reddit_decider-1.2.9/Cargo.toml
--rw-r--r--   0        0        0       66 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/.gitignore
--rw-r--r--   0        0        0      910 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/README.md
--rw-r--r--   0        0        0       34 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/__init__.py
--rw-r--r--   0        0        0       76 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/pyproject.toml
--rw-r--r--   0        0        0       40 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/setup.cfg
--rw-r--r--   0        0        0     1284 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/setup.py
--rw-r--r--   0        0        0    20979 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/src/lib.rs
--rw-r--r--   0        0        0       66 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/test/.gitignore
--rw-r--r--   0        0        0    10110 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/test/integration_test.py
--rw-r--r--   0        0        0       93 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/test/requirements.txt
--rw-r--r--   0        0        0     2903 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/test/test_rust.py
--rw-r--r--   0        0        0    33983 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/test/unit_test.py
--rw-r--r--   0        0        0     3088 2022-07-05 23:23:03.000000 reddit_decider-1.2.9/test/utils.py
--rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 reddit_decider-1.2.9/PKG-INFO
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 reddit_decider-1.3.0/local_dependencies/decider/Cargo.toml
+-rw-r--r--   0        0        0       19 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/local_dependencies/decider/.gitignore
+-rw-r--r--   0        0        0      323 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/local_dependencies/decider/Makefile
+-rw-r--r--   0        0        0      710 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/local_dependencies/decider/README.md
+-rw-r--r--   0        0        0     6097 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/local_dependencies/decider/benches/decider.rs
+-rw-r--r--   0        0        0     9514 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/local_dependencies/decider/src/context.rs
+-rw-r--r--   0        0        0    48183 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/local_dependencies/decider/src/events.rs
+-rw-r--r--   0        0        0   108868 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/local_dependencies/decider/src/lib.rs
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 reddit_decider-1.3.0/Cargo.toml
+-rw-r--r--   0        0        0      112 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/.gitignore
+-rw-r--r--   0        0        0      786 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/Makefile
+-rw-r--r--   0        0        0     6041 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/README.md
+-rw-r--r--   0        0        0      273 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    22412 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/python/rust_decider/__init__.py
+-rw-r--r--   0        0        0      259 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/python/rust_decider/prometheus_metrics.py
+-rw-r--r--   0        0        0      177 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/requirements-dev.txt
+-rw-r--r--   0        0        0       40 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/setup.cfg
+-rw-r--r--   0        0        0     1300 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/setup.py
+-rw-r--r--   0        0        0    34812 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/src/lib.rs
+-rw-r--r--   0        0        0    39025 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/test/decider_unit_test.py
+-rw-r--r--   0        0        0    10110 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/test/integration_test.py
+-rw-r--r--   0        0        0     2903 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/test/test_rust.py
+-rw-r--r--   0        0        0    34104 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/test/unit_test.py
+-rw-r--r--   0        0        0     3088 2023-06-07 08:40:12.000000 reddit_decider-1.3.0/test/utils.py
+-rw-r--r--   0        0        0     6238 1970-01-01 00:00:00.000000 reddit_decider-1.3.0/PKG-INFO
```

### Comparing `reddit_decider-1.2.9/local_dependencies/decider/Cargo.toml` & `reddit_decider-1.3.0/local_dependencies/decider/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [package]
 name = "decider"
-version = "1.2.9"
+version = "1.3.0"
 edition = "2021"
 description = "a package for AB-testing and dynamic config"
 homepage = "https://mattknox.com"
 license = "MIT"
 documentation = "https://mattknox.com/decider"
 readme = "README.md"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 chrono = "0.4"
 float-cmp = "0.9"
 num-bigint = "^0.4"
 rand = "0.8.3"
-rust-crypto = "^0.2"
 serde = { version = "1.0", features = ["derive"] }
 serde_json = "^1.0.59"
+sha-1 = "0.10"
+thiserror = "1.0"
 uuid = { version = "1.1", features = ["serde", "v4"] }
 
 [dev-dependencies]
 proptest = "1.0.0" # check this out at https://altsysrq.github.io/proptest-book/intro.html
 criterion = { version = "0.3", features = ["html_reports"] }
 
 [lib]
```

### Comparing `reddit_decider-1.2.9/local_dependencies/decider/README.md` & `reddit_decider-1.3.0/local_dependencies/decider/README.md`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.2.9/local_dependencies/decider/benches/decider.rs` & `reddit_decider-1.3.0/local_dependencies/decider/benches/decider.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use criterion::measurement::WallTime;
 use criterion::{
     black_box, criterion_group, criterion_main, BenchmarkGroup, BenchmarkId, Criterion, Throughput,
 };
 use std::collections::HashMap;
 use std::path::PathBuf;
 
-use decider::{init_decider, BucketVal, Context, Decider};
+use decider::{init_decider, Context, ContextField, Decider};
 
 const DECIDER_CFG: &str =
     "darkmode overrides targeting holdout mutex_group fractional_availability value";
 
 fn resource_path(file: &str) -> String {
     let mut dir = PathBuf::from(env!("CARGO_MANIFEST_DIR"));
     dir.pop();
@@ -194,24 +194,22 @@
     group.throughput(Throughput::Elements(1));
 
     let decider = init_decider(DECIDER_CFG, &resource_path("bench_cfg.json")).unwrap();
     let ctx = Context::default();
 
     for (bv_str, bv) in vec![
         ("none", None),
-        ("user_id", Some(BucketVal::UserId)),
-        ("device_id", Some(BucketVal::DeviceId)),
-        ("canonical_url", Some(BucketVal::CanonicalUrl)),
-    ] {
+        ("user_id", Some(ContextField::UserId)),
+        ("device_id", Some(ContextField::DeviceId)),
+        ("canonical_url", Some(ContextField::CanonicalUrl)),
+    ]
+    .into_iter()
+    {
         group.bench_function(format!("choose_all/bv_override_{}", bv_str), |b| {
-            b.iter(|| {
-                decider
-                    .choose_all(black_box(&ctx), black_box(bv.clone()))
-                    .unwrap();
-            })
+            b.iter(|| decider.choose_all(black_box(&ctx), black_box(bv.clone())))
         });
     }
 }
 
 criterion_group!(
     benches,
     bench_dynamic_config,
```

### Comparing `reddit_decider-1.2.9/local_dependencies/decider/src/events.rs` & `reddit_decider-1.3.0/local_dependencies/decider/src/events.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,125 +1,119 @@
 use chrono::Utc;
 use std::error::Error;
 use std::fmt::{Debug, Display, Formatter};
 use std::num::TryFromIntError;
 
-use crate::Event as DecisionEvent;
-use crate::{BucketVal, Context, DecisionKind};
+use crate::{Context, DecisionKind};
+use crate::{ContextField, Event as DecisionEvent};
 use serde::ser::SerializeMap;
 use serde::{Serialize, Serializer};
 use uuid::Uuid;
 
 // Consts for the experiment SAN.
 const SOURCE: Thrifty<&'static str> = Thrifty {
     value: "experiment",
 };
 
 const ACTION: Thrifty<&'static str> = Thrifty { value: "expose" };
 
-const NOUN_USER_ID: Thrifty<&'static str> = Thrifty { value: "user_id" };
-const NOUN_DEVICE_ID: Thrifty<&'static str> = Thrifty { value: "device_id" };
-const NOUN_CANONICAL_URL: Thrifty<&'static str> = Thrifty {
-    value: "canonical_url",
-};
-
 /// `EventStrings` holds serialized strings representing exposure events.
 ///
 /// `event_data` use the legacy format: values are separated by "::::" and are parsed by the python
 /// client.
 ///
 /// `event_json` represents a fully hydrated thrift event that can be sent to the V2 events
-/// collector.  
+/// collector.
 pub(crate) struct SerializedEvents {
     pub(crate) event_data: Vec<String>,
     pub(crate) events: Vec<DecisionEvent>,
 }
 
 impl SerializedEvents {
     pub(crate) fn new(
         ctx: &Context,
         internal_events: Vec<ExperimentEvent>,
     ) -> Result<Self, Box<dyn Error>> {
         let client_timestamp = &Utc::now().timestamp_millis().into();
 
         // All events for a single decision share the same correlation id.
-        let correlation_id = &Uuid::new_v4().into();
+        let correlation_id = get_correlation_id(ctx).into();
 
         let app = &App::new(ctx).map(Thrifty::from);
         let platform = &Platform::new(ctx).map(Thrifty::from);
         let request = &Request::new(ctx).map(Thrifty::from);
+        let subreddit = &Subreddit::new(ctx).map(Thrifty::from);
         let user = &User::new(ctx).map(Thrifty::from);
         let geo = &Geo::new(ctx).map(Thrifty::from);
 
         let num_events = internal_events.len();
 
         internal_events
             .into_iter()
-            // For each event...
-            .map(|exp_ev| {
-                // First, hydrate the legacy format string.
-                let data_string = exp_ev.to_string();
-
-                let noun = match &exp_ev.bucketing_field {
-                    BucketVal::UserId => NOUN_USER_ID,
-                    BucketVal::DeviceId => NOUN_DEVICE_ID,
-                    BucketVal::CanonicalUrl => NOUN_CANONICAL_URL,
-                };
-
-                let kind = exp_ev.decision_kind;
-
-                // Then, try to create an experiment from the available pieces.
-                Experiment::try_from(exp_ev)
-                    .map(|exp| {
-                        let event = Event {
-                            source: SOURCE,
-                            action: ACTION,
-                            noun,
-                            client_timestamp,
-                            uuid: Uuid::new_v4().into(),
-                            correlation_id,
-                            app,
-                            platform,
-                            request,
-                            user,
-                            experiment: exp.into(),
-                            geo,
-                        };
-                        (data_string, kind, event)
-                    })
-                    // Box any errors to unify with the serde errors in the fold.
-                    .map_err(|err| err.into())
-            })
             // Roll the results up into the holder struct. `try_fold` will return early if it
             // encounters an error.
-            .try_fold::<_, _, Result<SerializedEvents, Box<dyn Error>>>(
+            .try_fold(
                 SerializedEvents {
                     event_data: Vec::with_capacity(num_events),
                     events: Vec::with_capacity(num_events),
                 },
-                |mut acc, event_res: Result<(String, DecisionKind, Event<'_>), Box<dyn Error>>| {
-                    let (data_string, kind, event) = event_res?;
-                    acc.event_data.push(data_string);
-
-                    let json_string = serde_json::to_string(&event)
-                        .map_err::<Box<dyn Error>, _>(|err| err.into())?;
+                |mut acc, exp_ev| {
+                    // First, hydrate the legacy format string.
+                    let data_string = exp_ev.to_string();
+                    let noun = exp_ev.bucketing_field.to_string().into();
+                    let kind = exp_ev.decision_kind;
+                    let exposure_key = format!(
+                        "{}:{}:{}:{}",
+                        exp_ev.feature_name,
+                        exp_ev.feature_version,
+                        exp_ev.variant_name,
+                        exp_ev.bucketing_value,
+                    );
+
+                    // Then, try to create an experiment from the available pieces.
+                    let event = Event {
+                        source: SOURCE,
+                        action: ACTION,
+                        noun,
+                        client_timestamp,
+                        uuid: Uuid::new_v4().into(),
+                        correlation_id: &correlation_id,
+                        app,
+                        platform,
+                        request,
+                        subreddit,
+                        user,
+                        experiment: Experiment::try_from(exp_ev)?.into(),
+                        geo,
+                    };
 
                     let decision_event = DecisionEvent {
                         kind,
-                        json: json_string,
+                        exposure_key,
+                        json: serde_json::to_string(&event)?,
                     };
 
+                    acc.event_data.push(data_string);
                     acc.events.push(decision_event);
 
                     Ok(acc)
-                },
+                }
             )
     }
 }
 
+fn get_correlation_id(ctx: &Context) -> Uuid {
+    // If the correlation id is set, try to parse it as a Uuid. If the value is missing or not a
+    // Uuid, generate one instead.
+    ctx.correlation_id
+        .as_ref()
+        .and_then(|sval| Uuid::try_parse(sval).ok())
+        .unwrap_or_else(Uuid::new_v4)
+}
+
 /// `Event` is a serde proxy for the V2 event struct. Note that in order to avoid a dependency on
 /// thrift, this struct is its own minimal version of the TJsonProtocol.
 ///
 /// The thrift JSON protocol uses the field indices as json map keys, and encodes all types as
 /// objects:
 /// - Strings are encoded as `{"str": $value}`.
 /// - Integers are encoded as `{"i32": $value}`, or `{"i64": $value}`.
@@ -140,18 +134,17 @@
     #[serde(rename = "1")]
     source: Thrifty<&'static str>,
 
     // Action is always "expose".
     #[serde(rename = "2")]
     action: Thrifty<&'static str>,
 
-    // Noun is one of: "user_id", "device_id", or "canonical_url", depending on the bucketing field
-    // of the returned event.
+    // Noun is the name of the bucketing field of the returned event.
     #[serde(rename = "3")]
-    noun: Thrifty<&'static str>,
+    noun: Thrifty<String>,
 
     // An arbitrary timestamp of when these events are generated.
     #[serde(rename = "5")]
     client_timestamp: &'ev Thrifty<i64>,
 
     // A random Uuid.
     #[serde(rename = "6")]
@@ -170,14 +163,17 @@
 
     #[serde(rename = "109", skip_serializing_if = "Option::is_none")]
     request: &'ev Option<Thrifty<Request<'ev>>>,
 
     #[serde(rename = "112", skip_serializing_if = "Option::is_none")]
     user: &'ev Option<Thrifty<User<'ev>>>,
 
+    #[serde(rename = "114", skip_serializing_if = "Option::is_none")]
+    subreddit: &'ev Option<Thrifty<Subreddit<'ev>>>,
+
     #[serde(rename = "129")]
     experiment: Thrifty<Experiment>,
 
     #[serde(rename = "500", skip_serializing_if = "Option::is_none")]
     geo: &'ev Option<Thrifty<Geo<'ev>>>,
 }
 
@@ -241,14 +237,32 @@
             Some(Platform {
                 device_id: uuid.into(),
             })
         })
     }
 }
 
+/// The `Subreddit` substruct of the V2 event. The schema is available
+/// [here](https://github.snooguts.net/reddit/data-schemas/blob/master/schemas/components/subreddit.thrift#L14).
+#[derive(Clone, Debug, Serialize)]
+struct Subreddit<'a> {
+    // Extracted from `Context.subreddit_id`. Since this is the only field we set on the substruct, the
+    // entire substruct is elided if it's not set on the context.
+    #[serde(rename = "1")]
+    id: Thrifty<&'a str>,
+}
+
+impl Subreddit<'_> {
+    fn new(ctx: &Context) -> Option<Subreddit<'_>> {
+        ctx.subreddit_id.as_ref().map(|s_id| Subreddit {
+            id: s_id.as_str().into(),
+        })
+    }
+}
+
 /// The `Request` substruct of the V2 event. The schema is available
 /// [here](https://github.snooguts.net/reddit/data-schemas/blob/master/schemas/components/request.thrift#L9).
 #[derive(Clone, Debug, Serialize)]
 struct Request<'a> {
     // Extracted from `Context.canonical_url`. Since this is the only field we set on the substruct,
     // the entire substruct is elided if it's not set on the context.
     #[serde(rename = "17")]
@@ -351,15 +365,15 @@
     fn try_from(value: ExperimentEvent) -> Result<Self, Self::Error> {
         let experiment_id = i64::from(value.feature_id).into();
         let name = value.feature_name.into();
         let owner = value.owner.into();
         let variant = value.variant_name.into();
         let start_ts = i64::try_from(value.start_ts)?.into();
         let stop_ts = i64::try_from(value.stop_ts)?.into();
-        let bucketing_key = value.bucketing_field.to_string().into();
+        let bucketing_key = String::from(value.bucketing_field).into();
         let version = value.feature_version.to_string().into();
         let bucketing_value = value.bucketing_value.into();
         let is_override = (value.decision_kind == DecisionKind::Override).into();
 
         Ok(Experiment {
             experiment_id,
             name,
@@ -398,15 +412,15 @@
 #[derive(Clone, Debug)]
 pub(crate) struct ExperimentEvent {
     pub(crate) decision_kind: DecisionKind,
     pub(crate) feature_id: u32,
     pub(crate) feature_name: String,
     pub(crate) feature_version: u32,
     pub(crate) variant_name: String,
-    pub(crate) bucketing_field: BucketVal,
+    pub(crate) bucketing_field: ContextField,
     pub(crate) bucketing_value: String,
     pub(crate) start_ts: u64,
     pub(crate) stop_ts: u64,
     pub(crate) owner: String,
 }
 
 // TODO Remove this trait once we've migrated off the legacy string format.
@@ -418,15 +432,15 @@
             "{}::::{}::::{}::::{}::::{}::::{}::::{}::::{}::::{}::::{}",
             self.decision_kind as u8,
             self.feature_id,
             self.feature_name,
             self.feature_version,
             self.variant_name,
             self.bucketing_value,
-            self.bucketing_field,
+            self.bucketing_field.as_ref(),
             self.start_ts,
             self.stop_ts,
             self.owner,
         )
     }
 }
 
@@ -450,15 +464,15 @@
         impl_tagged!($tag, [$typ]);
     };
 }
 
 impl_tagged!("str", [&str, String, Uuid]);
 impl_tagged!("i32", i32);
 impl_tagged!("i64", i64);
-impl_tagged!("rec", [App<'_>, Experiment, Geo<'_>, Platform, Request<'_>, User<'_>]);
+impl_tagged!("rec", [App<'_>, Experiment, Geo<'_>, Platform, Request<'_>, Subreddit<'_>, User<'_>]);
 
 /// `Thrifty` is a wrapper that ensures values are encoded using the thrift json protocol. When `T`
 /// is `Serializable + Tagged`, `Thrifty<T>` is encoded as `{$tag: $value}`.
 ///
 /// Note that thrift bools are encoded as integers with a custom tag, and so have a wholly unique
 /// `Serialize` implementation.
 struct Thrifty<T> {
@@ -507,24 +521,20 @@
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "Thrifty {{ value: {:?} }}", self.value)
     }
 }
 
 #[cfg(test)]
 mod tests {
-    use prop::option;
-    use prop::strategy::Strategy;
+    use crate::{DecisionKind, ExperimentEvent};
     use proptest::prelude::*;
-    use uuid::Uuid;
-
-    use crate::{BucketVal, Context, DecisionKind, ExperimentEvent};
 
     pub(super) mod app {
         use super::super::*;
-        use super::context_strategy;
+        use crate::generators::context_strategy;
         use prop::option;
         use proptest::prelude::*;
         use serde_json::{json, Value};
 
         proptest! {
             #[test]
             fn test_new(ctx in context_strategy()) {
@@ -594,14 +604,15 @@
             }
         }
     }
 
     pub(super) mod platform {
         use super::super::*;
         use super::*;
+        use crate::generators::*;
         use serde_json::{json, Value};
 
         proptest! {
             #[test]
             fn test_new_bad_uuid(mut ctx in context_strategy(), uuid in ".*") {
                 ctx.device_id = Some(uuid);
 
@@ -646,17 +657,64 @@
                 });
 
                 (platform, expected_value)
             }
         }
     }
 
+    pub(super) mod subreddit {
+        use super::super::*;
+        use super::*;
+        use crate::generators::*;
+        use serde_json::{json, Value};
+
+        proptest! {
+            #[test]
+            fn test_new(ctx in context_strategy()) {
+                let subreddit = Subreddit::new(&ctx);
+
+                if ctx.subreddit_id.is_none() {
+                    prop_assert!(subreddit.is_none());
+                } else {
+                    prop_assert!(subreddit.is_some());
+                    let expected_sr_id = &ctx.subreddit_id.clone().unwrap();
+                    prop_assert_eq!(expected_sr_id, subreddit.unwrap().id.value);
+                }
+            }
+
+            #[test]
+            fn test_serialize((subreddit, expected_value) in subreddit_strategy()) {
+                let serialized = serde_json::to_value(subreddit).unwrap();
+                prop_assert_eq!(expected_value, serialized);
+            }
+        }
+
+        prop_compose! {
+            pub(super) fn subreddit_strategy()(
+                subreddit_id in ".*",
+            ) -> (Subreddit<'static>, Value) {
+                let subreddit_id_str: &'static str = Box::leak(subreddit_id.clone().into_boxed_str());
+                let subreddit = Subreddit {
+                    id: subreddit_id_str.into(),
+                };
+
+                let expected_value = json!({
+                    "1": {
+                        "str": subreddit_id_str.to_string(),
+                    }
+                });
+
+                (subreddit, expected_value)
+            }
+        }
+    }
+
     pub(super) mod request {
         use super::super::*;
-        use super::context_strategy;
+        use crate::generators::context_strategy;
         use proptest::prelude::*;
         use serde_json::{json, Value};
 
         proptest! {
             #[test]
             fn test_new(ctx in context_strategy()) {
                 let request = Request::new(&ctx);
@@ -698,15 +756,15 @@
                 (request, expected_value)
             }
         }
     }
 
     pub(super) mod user {
         use super::super::*;
-        use super::context_strategy;
+        use crate::generators::context_strategy;
         use prop::option;
         use proptest::prelude::*;
         use serde_json::{json, Value};
 
         proptest! {
             #[test]
             fn test_new(ctx in context_strategy()) {
@@ -775,14 +833,15 @@
         }
     }
 
     pub(super) mod experiment {
         use super::super::*;
         use super::experiment_event::experiment_event_strategy;
         use super::*;
+        use crate::generators::bucketing_field;
         use serde_json::{json, Value};
 
         proptest! {
             #[test]
             fn test_try_from_invalid_start(mut event in experiment_event_strategy(), start_ts in (i64::MAX as u64)..) {
                 event.start_ts = start_ts;
 
@@ -827,15 +886,15 @@
             pub(super) fn experiment_strategy()(
                 experiment_id in prop::num::i64::ANY,
                 name in ".*",
                 owner in ".*",
                 variant in ".*",
                 start_ts in prop::num::i64::ANY,
                 stop_ts in prop::num::i64::ANY,
-                bucketing_field in bucket_val(),
+                bucketing_field in bucketing_field(),
                 version in ".*",
                 bucketing_value in ".*",
                 is_override in prop::bool::ANY,
             ) -> (Experiment, Value) {
                 let bucketing_key = bucketing_field.to_string();
 
                 let exp = Experiment {
@@ -887,15 +946,15 @@
                 (exp, expected_value)
             }
         }
     }
 
     pub(super) mod geo {
         use super::super::*;
-        use super::context_strategy;
+        use crate::generators::context_strategy;
         use proptest::prelude::*;
         use serde_json::{json, Value};
 
         proptest! {
             #[test]
             fn test_new(ctx in context_strategy()) {
                 let geo = Geo::new(&ctx);
@@ -937,14 +996,15 @@
                 (geo, expected_value)
             }
         }
     }
 
     pub(super) mod experiment_event {
         use super::*;
+        use crate::generators::*;
 
         proptest! {
             #[test]
             fn test_to_string(event in experiment_event_strategy()) {
                 let event_str = event.to_string();
                 let mut tokens = event_str.split("::::");
 
@@ -981,15 +1041,15 @@
         prop_compose! {
             pub(super) fn experiment_event_strategy() (
                 decision_kind in decision_kind(),
                 feature_id in prop::num::u32::ANY,
                 feature_name in "[^:]*",
                 feature_version in prop::num::u32::ANY,
                 variant_name in "[^:]*",
-                bucketing_field in bucket_val(),
+                bucketing_field in bucketing_field(),
                 bucketing_value in "[^:]*",
                 start_ts in 0u64..=(i64::MAX as u64),
                 stop_ts in 0u64..=(i64::MAX as u64),
                 owner in "[^:]*",
             ) -> ExperimentEvent {
                 ExperimentEvent {
                     decision_kind,
@@ -1006,17 +1066,17 @@
             }
         }
     }
 
     mod event {
         use super::super::*;
         use super::*;
+        use crate::generators::uuid;
         use prop::option;
         use serde_json::{json, Value};
-        use std::str::FromStr;
 
         proptest! {
             #[test]
             fn test_serialize((event, expected_value) in event_strategy()) {
                 let serialized = serde_json::to_value(event).unwrap();
 
                 prop_assert_eq!(expected_value, serialized);
@@ -1027,26 +1087,24 @@
             fn event_strategy()(
                 client_timestamp in prop::num::i64::ANY,
                 uuid in uuid(),
                 correlation_id in uuid(),
                 app_opt in option::of(app::app_strategy()),
                 platform_opt in option::of(platform::platform_strategy()),
                 request_opt in option::of(request::request_strategy()),
+                subreddit_opt in option::of(subreddit::subreddit_strategy()),
                 user_opt in option::of(user::user_strategy()),
                 (experiment, expected_exp_value) in experiment::experiment_strategy(),
                 geo_opt in option::of(geo::geo_strategy()),
             ) -> (Event<'static>, Value) {
                 let client_timestamp: &'static Thrifty<i64> = Box::leak(Box::new(client_timestamp.into()));
                 let correlation_id: &'static Thrifty<Uuid> = Box::leak(Box::new(correlation_id.into()));
 
-                let (noun, expected_noun_str) = match BucketVal::from_str(&experiment.bucketing_key.value).unwrap() {
-                    BucketVal::UserId => (NOUN_USER_ID, "user_id"),
-                    BucketVal::DeviceId => (NOUN_DEVICE_ID, "device_id"),
-                    BucketVal::CanonicalUrl => (NOUN_CANONICAL_URL, "canonical_url"),
-                };
+                let noun = experiment.bucketing_key.clone();
+                let expected_noun_str = noun.value.clone();
 
                 let (app, expected_app_value) = match app_opt {
                     Some((a, v)) => {
                         let boxed: &'static Option<Thrifty<App<'static>>> = Box::leak(Box::new(Some(a.into())));
 
                         (boxed, Some(v))
                     },
@@ -1058,14 +1116,23 @@
                         let boxed: &'static Option<Thrifty<Platform>> = Box::leak(Box::new(Some(p.into())));
 
                         (boxed, Some(v))
                     },
                     _ => (&None, None),
                 };
 
+                let (subreddit, expected_subreddit_value) = match subreddit_opt {
+                    Some((p, v)) => {
+                        let boxed: &'static Option<Thrifty<Subreddit<'static>>> = Box::leak(Box::new(Some(p.into())));
+
+                        (boxed, Some(v))
+                    },
+                    _ => (&None, None),
+                };
+
                 let (request, expected_request_value) = match request_opt {
                     Some((r, v)) => {
                         let boxed: &'static Option<Thrifty<Request<'static>>> = Box::leak(Box::new(Some(r.into())));
 
                         (boxed, Some(v))
                     },
                     _ => (&None, None),
@@ -1095,14 +1162,15 @@
                     noun,
                     client_timestamp,
                     uuid: uuid.into(),
                     correlation_id,
                     app,
                     platform,
                     request,
+                    subreddit,
                     user,
                     experiment: experiment.into(),
                     geo,
                 };
 
                 let mut expected_value = json!({
                     "1": {
@@ -1134,14 +1202,19 @@
                     }));
                 }
                 if let Some(epv) = expected_platform_value {
                     expected_value.as_object_mut().unwrap().insert("108".to_string(), json!({
                         "rec": epv,
                     }));
                 }
+                if let Some(esv) = expected_subreddit_value {
+                    expected_value.as_object_mut().unwrap().insert("114".to_string(), json!({
+                        "rec": esv,
+                    }));
+                }
                 if let Some(erv) = expected_request_value {
                     expected_value.as_object_mut().unwrap().insert("109".to_string(), json!({
                         "rec": erv,
                     }));
                 }
                 if let Some(euv) = expected_user_value {
                     expected_value.as_object_mut().unwrap().insert("112".to_string(), json!({
@@ -1158,14 +1231,15 @@
             }
         }
     }
 
     mod serialized_events {
         use super::super::*;
         use super::*;
+        use crate::generators::context_strategy;
         use chrono::{TimeZone, Utc};
         use serde_json::{json, Map, Value};
 
         proptest! {
             #[test]
             fn test_new(
                 ctx in context_strategy(),
@@ -1175,26 +1249,37 @@
                 let parsed_events = SerializedEvents::new(&ctx, vec![event.clone()]).unwrap();
                 let expected_data_string = event.to_string();
 
                 prop_assert_eq!(vec![expected_data_string], parsed_events.event_data);
 
                 prop_assert_eq!(1, parsed_events.events.len());
                 prop_assert_eq!(event.decision_kind, parsed_events.events[0].kind);
+
+                let expected_exposure_key = format!(
+                    "{}:{}:{}:{}",
+                    event.feature_name,
+                    event.feature_version,
+                    event.variant_name,
+                    event.bucketing_value,
+                );
+                prop_assert_eq!(&expected_exposure_key, &parsed_events.events[0].exposure_key);
+
                 let parsed: Value = serde_json::from_str(&parsed_events.events[0].json).unwrap();
                 let jv: &Map<String, Value> = parsed.as_object().unwrap();
 
                 prop_assert_eq!(&json!("experiment"), &jv["1"]["str"]);
                 prop_assert_eq!(&json!("expose"), &jv["2"]["str"]);
 
                 let actual_noun = &jv["3"]["str"];
 
                 match event.bucketing_field {
-                    BucketVal::UserId => prop_assert_eq!(&json!("user_id"), actual_noun),
-                    BucketVal::DeviceId => prop_assert_eq!(&json!("device_id"), actual_noun),
-                    BucketVal::CanonicalUrl => prop_assert_eq!(&json!("canonical_url"), actual_noun),
+                    ContextField::UserId => prop_assert_eq!(&json!("user_id"), actual_noun),
+                    ContextField::DeviceId => prop_assert_eq!(&json!("device_id"), actual_noun),
+                    ContextField::CanonicalUrl => prop_assert_eq!(&json!("canonical_url"), actual_noun),
+                    _ => unreachable!("TODO expand tests to include all context fields"),
                 };
 
                 let event_ts = &jv["5"]["i64"].as_i64().unwrap();
                 let event_time = Utc.timestamp_millis(*event_ts);
                 prop_assert!((event_time - now).num_milliseconds().abs() < 1000);
 
                 // UUIDs are unique, so just check for presence.
@@ -1228,63 +1313,8 @@
                     None => prop_assert!(&jv.get("500").is_none()),
                 }
 
                 prop_assert_eq!(&Value::from(event.feature_id), &jv["129"]["rec"]["1"]["i64"]);
             }
         }
     }
-
-    prop_compose! {
-        fn context_strategy()(
-            user_id in option::of(".*"),
-            locale in option::of(".*"),
-            country_code in option::of(".*"),
-            device_id in option::of(uuid()),
-            canonical_url in option::of(".*"),
-            origin_service in option::of(".*"),
-            user_is_employee in option::of(prop::bool::ANY),
-            logged_in in option::of(prop::bool::ANY),
-            app_name in option::of(".*"),
-            build_number in option::of(prop::num::i32::ANY),
-            auth_client_id in option::of(".*"),
-            cookie_created_timestamp in option::of(prop::num::i64::ANY),
-            // other_fields omitted for sanity
-        ) -> Context {
-            let device_id = device_id.map(|uuid| uuid.to_string());
-            Context {
-                user_id,
-                locale,
-                country_code,
-                device_id,
-                canonical_url,
-                origin_service,
-                user_is_employee,
-                logged_in,
-                app_name,
-                build_number,
-                auth_client_id,
-                cookie_created_timestamp,
-                other_fields: None,
-            }
-        }
-    }
-
-    fn uuid() -> impl Strategy<Value = Uuid> {
-        Just(Uuid::new_v4())
-    }
-
-    fn decision_kind() -> impl Strategy<Value = DecisionKind> {
-        let options: Vec<_> = (0u8..)
-            .map_while(|v| DecisionKind::try_from(v).ok())
-            .collect();
-
-        prop::sample::select(options)
-    }
-
-    fn bucket_val() -> impl Strategy<Value = BucketVal> {
-        prop::sample::select(vec![
-            BucketVal::UserId,
-            BucketVal::DeviceId,
-            BucketVal::CanonicalUrl,
-        ])
-    }
 }
```

### Comparing `reddit_decider-1.2.9/local_dependencies/decider/src/lib.rs` & `reddit_decider-1.3.0/local_dependencies/decider/src/lib.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,270 +1,204 @@
 #![warn(rust_2018_idioms)]
 
 //! Decider is a library for determining whether a given feature should be available
 //! in a given context.  It supports a very expressive set of operations for determining
 //! which features should be available (and in what variant, if more than one is desired)
 //! in a context.
+mod context;
 mod events;
 
+use std::borrow::Borrow;
 use std::collections::HashMap;
+use std::convert::identity;
 use std::error::Error;
 use std::fmt;
 use std::fs::File;
-use std::io::BufReader;
+use std::io::{BufReader, Read};
+use std::ops::{Not, Range};
 use std::path::Path;
-use std::str::FromStr;
 
 use crate::events::SerializedEvents;
-use crypto;
 use events::ExperimentEvent;
 use float_cmp::approx_eq;
 use num_bigint::BigUint;
 use serde::{Deserialize, Serialize};
 use serde_json::Value;
+use sha1::{Digest, Sha1};
+use thiserror::Error;
 
-use self::crypto::digest::Digest;
-use self::crypto::sha1::Sha1;
-
-/// A context captures the relevant state in which we want to find out whether a feature
-/// should be available.
-#[derive(Deserialize, Debug, Clone, Default)]
-pub struct Context {
-    pub user_id: Option<String>,
-
-    /// IETF language tag representing the preferred locale for the client, used for
-    /// providing localized content. Consists of an ISO 639-1 primary language subtag and
-    /// an optional ISO 3166-1 alpha-2 region subtag separated by an underscore.
-    ///
-    /// e.g. `en`, `en_US`.
-    pub locale: Option<String>,
-
-    /// A two-character ISO 3166-1 country code.
-    ///
-    /// e.g. `US`.
-    pub country_code: Option<String>,
-    pub device_id: Option<String>,
-    pub canonical_url: Option<String>,
-    pub origin_service: Option<String>,
-    pub user_is_employee: Option<bool>,
-    pub logged_in: Option<bool>,
-    pub app_name: Option<String>,
-    pub build_number: Option<i32>,
-    pub auth_client_id: Option<String>,
-    pub cookie_created_timestamp: Option<i64>,
-    pub other_fields: Option<HashMap<String, Value>>,
-}
-
-impl Context {
-    fn for_bucket_val(bv: &BucketVal, s: String) -> Context {
-        Context::default().with_bucket_val(bv, s)
-    }
-
-    fn with_bucket_val(&self, bucket_val: &BucketVal, s: String) -> Context {
-        let mut out = self.clone();
-        match bucket_val {
-            BucketVal::UserId => out.user_id = Some(s),
-            BucketVal::DeviceId => out.device_id = Some(s),
-            &BucketVal::CanonicalUrl => out.canonical_url = Some(s),
-        }
-        out
-    }
-
-    fn get_field(&self, field: &str) -> Result<Value, String> {
-        let v: Option<Value> = match field {
-            "user_id" => self.user_id.clone().map(Value::from),
-            "device_id" => self.device_id.clone().map(Value::from),
-            "canonical_url" => self.canonical_url.clone().map(Value::from),
-            "locale" => self.locale.clone().map(Value::from),
-            "country_code" => self.country_code.clone().map(Value::from),
-            "origin_service" => self.origin_service.clone().map(Value::from),
-            "app_name" => self.app_name.clone().map(Value::from),
-            "user_is_employee" => self.user_is_employee.map(Value::from),
-            "logged_in" => self.logged_in.map(Value::from),
-            "build_number" => self.build_number.map(Value::from),
-            "cookie_created_timestamp" => self.cookie_created_timestamp.map(Value::from),
-            "auth_client_id" => self.auth_client_id.clone().map(Value::from),
-            k => self.other_fields.as_ref().and_then(|m| m.get(k).cloned()),
-        };
-        v.ok_or(format!("missing field '{}'", field))
-    }
-
-    fn field_to_float(&self, name: &str) -> Result<f64, String> {
-        match self.get_field(name) {
-            Err(e) => Err(e),
-            Ok(Value::Number(n)) => match n.as_f64() {
-                None => Err("failed to get float".to_string()),
-                Some(f) => Ok(f),
-            },
-            Ok(Value::String(s)) => match s.parse::<f64>() {
-                Err(_) => Err("failed to parse string to float".to_string()),
-                Ok(f) => Ok(f),
-            },
-            Ok(v) => Err(format!("value '{}' not a String or Number", v)),
-        }
-    }
-
-    fn get_bucketing_field(&self, bucket_val: Option<&BucketVal>) -> Result<String, DeciderError> {
-        match bucket_val {
-            None => Err(DeciderError::MissingBucketVal),
-            Some(bv) => match bv {
-                BucketVal::UserId => match &self.user_id {
-                    Some(u_id) => Ok(u_id.clone()),
-                    None => Err(DeciderError::MissingBucketValInContext(
-                        "user_id".to_string(),
-                    )),
-                },
-                BucketVal::DeviceId => match &self.device_id {
-                    Some(d_id) => Ok(d_id.clone()),
-                    None => Err(DeciderError::MissingBucketValInContext(
-                        "device_id".to_string(),
-                    )),
-                },
-                BucketVal::CanonicalUrl => match &self.canonical_url {
-                    Some(c_url) => Ok(c_url.clone()),
-                    None => Err(DeciderError::MissingBucketValInContext(
-                        "canonical_url".to_string(),
-                    )),
-                },
-            },
-        }
-    }
-
-    fn cmp(&self, field: &str, value: &Value) -> Result<bool, String> {
-        match self.get_field(field) {
-            Err(e) => Err(e),
-            Ok(v) => value_eq(&v, value),
-        }
-    }
-
-    fn cmp_op(&self, comp: Comp, field_name: &str, value: f64) -> Result<bool, String> {
-        // GT/LT and friends only really make sense on Numbers, but sometimes might
-        // show up as Strings in the experiment_config.json
-        Ok(comp.cmp_floats(self.field_to_float(field_name)?, value))
-    }
-}
+pub use context::{Context, ContextField};
 
 /// Takes two [`Value`] references, possibly of different variants and compares them for equality.
 ///
 /// If one of the operands is a [`Value::String`] and the other is a [`Value::Number`], the string
 /// is parsed as a number before comparison.
 ///
 /// All numbers are treated as floats for comparison. The experiment config and the context's
 /// `other_fields` field are both json, which means comparing any two number values as integers may
 /// lead to subtly incorrect behavior. The downside is that float equality is approximate by
 /// definition. The values that we're expecting to compare, however, are small and imprecise enough
 /// that this shouldn't be a problem. For reference, we compare floats using the 64-bit
 /// [Machine epsilon](https://en.wikipedia.org/wiki/Machine_epsilon) and 4 [ULPs](https://en.wikipedia.org/wiki/Unit_in_the_last_place).
 ///
 /// For more information, see the [floating point comparison guide](https://floating-point-gui.de/errors/comparison/).
-fn value_eq(x: &Value, y: &Value) -> Result<bool, String> {
+fn value_eq(x: &Value, y: &Value) -> Option<bool> {
     match (&x, &y) {
-        (Value::Null, _) => Ok(y.is_null()),
-        (Value::Bool(b1), Value::Bool(b2)) => Ok(b1 == b2),
-        (Value::String(s1), Value::String(s2)) => Ok(s1 == s2),
+        (Value::Null, _) => Some(y.is_null()),
+        (Value::Bool(b1), Value::Bool(b2)) => Some(b1 == b2),
+        (Value::String(s1), Value::String(s2)) => Some(s1 == s2),
         (Value::String(s1), Value::Number(n2)) => {
             match (s1.parse::<f64>(), n2.as_f64()) {
-                (Ok(f1), Some(f2)) => Ok(approx_eq!(f64, f1, f2)),
+                (Ok(f1), Some(f2)) => Some(approx_eq!(f64, f1, f2)),
                 // s1 is not a parseable as number _or_ n2 is not convertible to f64. The latter
                 // should never happen.
-                _ => Ok(false),
+                _ => Some(false),
             }
         }
         (Value::Number(n1), Value::Number(n2)) => {
             match (n1.as_f64(), n2.as_f64()) {
-                (Some(f1), Some(f2)) => Ok(approx_eq!(f64, f1, f2)),
+                (Some(f1), Some(f2)) => Some(approx_eq!(f64, f1, f2)),
                 // Number(s) not convertible to float. Should never happen!
-                _ => Ok(false),
+                _ => Some(false),
             }
         }
         (Value::Number(n1), Value::String(s2)) => {
             match (n1.as_f64(), s2.parse::<f64>()) {
-                (Some(f1), Ok(f2)) => Ok(approx_eq!(f64, f1, f2)),
+                (Some(f1), Ok(f2)) => Some(approx_eq!(f64, f1, f2)),
                 // n1 is not convertible to float _or_ s2 is not parseable as a number. The former
                 // should never happen.
-                _ => Ok(false),
+                _ => Some(false),
             }
         }
-        _ => Err(format!("cannot compare '{:#?}' vs. '{:#?}'", x, y)),
+        _ => None,
     }
 }
 
-fn set_default_value(value_type: Option<&ValueType>) -> Value {
-    match value_type {
-        Some(vt) => match vt {
-            ValueType::Boolean => Value::Bool(false),
-            ValueType::Integer => Value::from(0),
-            ValueType::Float => Value::from(0.0),
-            ValueType::String => Value::from(""),
-            ValueType::Text => Value::from(""),
-            ValueType::Map => Value::Object(serde_json::Map::new()),
-        },
-        None => Value::Null,
-    }
+#[derive(Serialize, Deserialize, Debug, Clone)]
+pub struct Metadata {
+    pub id: u32,
+    pub name: String,
+    pub enabled: bool,
+    pub version: u32,
+    pub owner: String,
 }
 
-/// Features represent a unit of controllable code, that we might want to turn off, make
+#[derive(Serialize, Deserialize, Debug, Clone)]
+pub struct DynamicConfig {
+    metadata: Metadata,
+    value: Value,
+    value_type: ValueType,
+}
+
+/// RangeVariant represent a unit of controllable code, that we might want to turn off, make
 /// available only to some users, etc..  This is what FeatureFlags/AB tests control.
 #[derive(Serialize, Deserialize, Debug, Clone)]
-pub struct Feature {
-    id: u32,
-    name: String,
-    enabled: bool,
-    #[serde(rename(serialize = "type"))]
-    feature_type: ExperimentType,
-    version: u32,
-    owner: String,
-    emit_event: bool,
-    platform_bitmask: u64, // TODO: should this be made a vec for unbounded size?
-    value: Option<Value>,
-    value_type: Option<ValueType>,
+pub struct RangeVariant {
+    metadata: Metadata,
+    pub emit_event: bool,
+    pub variant_set: VariantSet,
+    enabled: bool, // is this just for darkmode?
     targeting: Option<TargetingTree>,
     overrides: Option<Vec<HashMap<String, TargetingTree>>>,
-    variant_set: Option<VariantSet>,
 }
 
-impl Feature {
+#[derive(Serialize, Deserialize, Debug, Clone)]
+pub enum Feature {
+    RangeVariant(RangeVariant),
+    DynamicConfig(DynamicConfig),
+}
+
+impl RangeVariant {
+    /// `get_variants` returns this feature's variants.
+    pub fn get_variants(&self) -> &Vec<Variant> {
+        &self.variant_set.variants
+    }
+
+    fn default_decision(&self, events: Vec<ExperimentEvent>) -> InternalDecision {
+        InternalDecision {
+            feature_id: self.metadata.id,
+            feature_name: self.metadata.name.clone(),
+            feature_version: self.metadata.version,
+            variant_name: None,
+            value: Value::Null,
+            value_type: None,
+            events,
+        }
+    }
+
     fn make_event(
         &self,
         dk: DecisionKind,
         variant_name: &str,
         ctx: &Context,
     ) -> Result<Option<ExperimentEvent>, DeciderError> {
         if !self.emit_event {
             return Ok(None);
         }
 
-        let variant_set = &self
+        let bucketing_value = self
             .variant_set
-            .as_ref()
-            .ok_or(DeciderError::MissingVariantSet)?;
-        let (bucketing_field, bucketing_value) = &variant_set
-            .bucket_val
+            .bucketing_field
+            .get_value(ctx)
             .ok_or(DeciderError::MissingBucketVal)
-            .and_then(|bucketing_field| {
-                let bucketing_value = ctx.get_bucketing_field(Some(&bucketing_field))?;
-                Ok((bucketing_field, bucketing_value))
+            .map(|v| match v {
+                // Json strings are formatted surrounded by quotes. Extract the inner value
+                // to avoid this.
+                Value::String(inner) => inner,
+                value => value.to_string(),
             })?;
 
         Ok(Some(ExperimentEvent {
             decision_kind: dk,
-            feature_id: self.id,
-            feature_name: self.name.clone(),
-            feature_version: self.version,
+            feature_id: self.metadata.id,
+            feature_name: self.metadata.name.clone(),
+            feature_version: self.metadata.version,
             variant_name: variant_name.to_string(),
-            bucketing_field: *bucketing_field,
-            bucketing_value: bucketing_value.clone(),
-            start_ts: variant_set.start_ts,
-            stop_ts: variant_set.stop_ts,
-            owner: self.owner.clone(),
+            bucketing_field: self.variant_set.bucketing_field.clone(),
+            bucketing_value,
+            start_ts: self.variant_set.start_ts,
+            stop_ts: self.variant_set.stop_ts,
+            owner: self.metadata.owner.clone(),
         }))
     }
 }
 
-#[derive(Copy, Clone, Debug, PartialEq, Eq)]
+impl DynamicConfig {
+    fn default_decision(&self, events: Vec<ExperimentEvent>) -> InternalDecision {
+        InternalDecision {
+            feature_id: self.metadata.id,
+            feature_name: self.metadata.name.clone(),
+            feature_version: self.metadata.version,
+            variant_name: None,
+            value: self.value.clone(),
+            value_type: Some(self.value_type),
+            events,
+        }
+    }
+}
+
+impl Feature {
+    pub fn metadata(&self) -> &Metadata {
+        match self {
+            Feature::RangeVariant(choice) => &choice.metadata,
+            Feature::DynamicConfig(dc) => &dc.metadata,
+        }
+    }
+
+    /// Returns a default decision for this feature. This is called when no decisionmaker
+    /// is able to make a decision on a feature.
+    fn default_decision(&self, events: Vec<ExperimentEvent>) -> InternalDecision {
+        match self {
+            Feature::RangeVariant(choice) => choice.default_decision(events),
+            Feature::DynamicConfig(dc) => dc.default_decision(events),
+        }
+    }
+}
+
+#[derive(Serialize, Copy, Clone, Debug, PartialEq, Eq)]
 pub enum DecisionKind {
     FracAvail = 0,
     Override = 1,
     Holdout = 2,
     MutexGroup = 3,
 }
 
@@ -286,96 +220,89 @@
             2 => Ok(Self::Holdout),
             3 => Ok(Self::MutexGroup),
             _ => Err(()),
         }
     }
 }
 
-/// VariantSet contains an experiment's variants, and all other fields not in common
-/// with dynamic config json.
-#[derive(Serialize, Deserialize, Debug, Clone)]
-struct VariantSet {
-    start_ts: u64, // TODO: consider whether this should just be created_at
-    stop_ts: u64,  // TODO: should we get rid of a version by creating a new one?
-    shuffle_version: u32,
-    bucket_val: Option<BucketVal>,
-    variants: Vec<Variant>,
-    holdout: Option<Box<Feature>>,
-    mutex_group: Option<Box<Feature>>,
-}
-
-/// Variants are primarily used for fractional availability, where, eg., 10% of users
-/// are exposed to a given version of a feature.
-#[derive(Serialize, Deserialize, Debug, Clone)]
-pub struct Variant {
-    name: String,
-    #[serde(rename = "range_start")] // TODO change to alias and remove
-    lo: f32, // consider changing away from floats.
-    #[serde(rename = "range_end")]
-    hi: f32,
-}
-
 #[derive(Serialize, Deserialize, Debug, Clone)]
 pub struct EqMany {
-    field: String,
+    field: ContextField,
     values: Vec<Value>,
 }
 
 impl EqMany {
-    fn eval(&self, ctx: &Context) -> Result<bool, String> {
-        let x = ctx.get_field(&self.field)?; // Let's not fetch lots of times.
-
-        self.values
-            .iter()
-            .map(|v| value_eq(&x, v))
-            .try_fold(false, |acc, res| Ok(acc || res?))
+    fn eval(&self, ctx: &Context) -> Option<bool> {
+        self.field.get_value(ctx).and_then(|x| {
+            self.values
+                .iter()
+                .map(|v| value_eq(&x, v))
+                .try_fold(false, |acc, res| res.map(|r| acc || r))
+        })
     }
 }
 
 #[derive(Serialize, Deserialize, Debug, Clone)]
 pub struct EqOne {
-    field: String,
+    field: ContextField,
     value: Value,
 }
 
 impl EqOne {
-    fn eval(&self, ctx: &Context) -> Result<bool, String> {
+    fn eval(&self, ctx: &Context) -> Option<bool> {
         ctx.cmp(&self.field, &self.value)
     }
 }
 
 #[derive(Serialize, Deserialize, Debug, Clone)]
 #[serde(untagged)]
 pub enum EqEnum {
     EqOne(EqOne),
     EqMany(EqMany),
 }
 
 impl EqEnum {
-    fn eval(&self, ctx: &Context) -> Result<bool, String> {
+    fn eval(&self, ctx: &Context) -> Option<bool> {
         match self {
             EqEnum::EqOne(eo) => eo.eval(ctx),
             EqEnum::EqMany(em) => em.eval(ctx),
         }
     }
 }
 
 /// The TargetingTree allows for arbitrary targeting operations, which can be used to
 /// limit an experiment to employees, or users from New Zealand, only to iOS users, etc...
+#[allow(clippy::upper_case_acronyms)]
 #[derive(Serialize, Deserialize, Debug, Clone)]
-pub enum TargetingTree {
+enum TargetingTree {
     ALL(Vec<TargetingTree>),
     ANY(Vec<TargetingTree>),
     NOT(Box<TargetingTree>),
+
     EQ(EqEnum),
-    GT { field: String, value: f64 },
-    LT { field: String, value: f64 },
-    GE { field: String, value: f64 },
-    LE { field: String, value: f64 },
-    NE { field: String, value: Value },
+    NE { field: ContextField, value: Value },
+
+    GT { field: ContextField, value: f64 },
+    LT { field: ContextField, value: f64 },
+    GE { field: ContextField, value: f64 },
+    LE { field: ContextField, value: f64 },
+}
+
+#[derive(Deserialize, Debug, Clone)]
+struct OverrideGroupFeature {
+    #[serde(rename = "value")]
+    groups: HashMap<String, OverrideGroup>,
+}
+
+#[derive(Deserialize, Debug, Clone)]
+struct OverrideGroup {
+    #[allow(dead_code)]
+    name: String,
+    values: Vec<Value>,
+    field: ContextField,
 }
 
 enum Comp {
     GT,
     LT,
     GE,
     LE,
@@ -388,139 +315,268 @@
             Comp::LT => f1 < f2,
             Comp::GE => f1 > f2 || approx_eq!(f64, f1, f2),
             Comp::LE => f1 < f2 || approx_eq!(f64, f1, f2),
         }
     }
 }
 impl TargetingTree {
-    fn eval(&self, ctx: &Context) -> Result<bool, String> {
+    fn eval(&self, ctx: &Context) -> Option<bool> {
         match self {
-            TargetingTree::ALL(xs) => {
-                let items: Result<Vec<bool>, String> = xs.iter().map(|x| x.eval(ctx)).collect();
-                Ok(items?.iter().all(|&b| b))
-            }
-            TargetingTree::ANY(xs) => {
-                let items: Result<Vec<bool>, String> = xs.iter().map(|x| x.eval(ctx)).collect();
-                Ok(items?.iter().any(|&b| b))
-            }
-            TargetingTree::NOT(x) => Ok(!(x.eval(ctx)?)),
+            TargetingTree::ALL(xs) => Some(
+                xs.iter()
+                    .map(|x| x.eval(ctx).unwrap_or(false))
+                    .all(identity),
+            ),
+            TargetingTree::ANY(xs) => Some(
+                // N.B. `ANY` uses `flat_map` which filters out `None` results. This is to allow
+                // ANY targeting to succeed in case some subset of targeted fields is missing in the
+                // context. `Iter::any` returns `false` on an empty iterator.
+                xs.iter().flat_map(|x| x.eval(ctx)).any(identity),
+            ),
+
             TargetingTree::EQ(es) => es.eval(ctx),
+            TargetingTree::NOT(x) => x.eval(ctx).map(Not::not),
+
             TargetingTree::GT { field, value } => ctx.cmp_op(Comp::GT, field, *value),
             TargetingTree::LT { field, value } => ctx.cmp_op(Comp::LT, field, *value),
             TargetingTree::GE { field, value } => ctx.cmp_op(Comp::GE, field, *value),
             TargetingTree::LE { field, value } => ctx.cmp_op(Comp::LE, field, *value),
-            TargetingTree::NE { field, value } => Ok(!(ctx.cmp(field, value)?)),
+
+            TargetingTree::NE { field, value } => ctx.cmp(field, value).map(Not::not),
+        }
+    }
+
+    /// Unrolls override groups in the targeting tree, replacing any references
+    /// to group values with the values specified in the group definition.
+    /// The `groups` parameter is a `HashMap` that maps group names to
+    /// `OverrideGroup` structs. This function returns a new `TargetingTree`
+    /// with the override groups unrolled.
+    ///
+    /// # Arguments
+    ///
+    /// * `self` - A reference to the current TargetingTree.
+    /// * `groups` - A reference to a HashMap of override group names to
+    /// `OverrideGroup` structs.
+    ///
+    fn unroll_groups(&self, groups: &HashMap<String, OverrideGroup>) -> Self {
+        let get_group = |value: &Value| -> Option<&OverrideGroup> {
+            groups.get(value.as_str().unwrap_or_default())
+        };
+
+        match self {
+            TargetingTree::ALL(trees) => {
+                TargetingTree::ALL(trees.iter().map(|t| t.unroll_groups(groups)).collect())
+            }
+            TargetingTree::ANY(trees) => {
+                TargetingTree::ANY(trees.iter().map(|t| t.unroll_groups(groups)).collect())
+            }
+            TargetingTree::NOT(tree) => TargetingTree::NOT(Box::new(tree.unroll_groups(groups))),
+            TargetingTree::EQ(eq) => match eq {
+                EqEnum::EqOne(one) => match get_group(&one.value) {
+                    Some(og) if og.field == one.field => {
+                        TargetingTree::EQ(EqEnum::EqMany(EqMany {
+                            field: og.field.clone(),
+                            values: og.values.clone(),
+                        }))
+                    }
+                    _ => self.clone(),
+                },
+                EqEnum::EqMany(many) => TargetingTree::EQ(EqEnum::EqMany(EqMany {
+                    field: many.field.clone(),
+                    values: many.values.iter().fold(vec![], |mut acc, v| {
+                        match get_group(v) {
+                            Some(og) => acc.extend(og.values.clone()),
+                            _ => acc.push(v.clone()),
+                        };
+                        acc
+                    }),
+                })),
+            },
+            TargetingTree::NE { field, value } => match get_group(value) {
+                Some(og) if &og.field == field => TargetingTree::ALL(
+                    og.values
+                        .iter()
+                        .map(|v| TargetingTree::NE {
+                            field: field.clone(),
+                            value: v.clone(),
+                        })
+                        .collect(),
+                ),
+                _ => self.clone(),
+            },
+            _ => self.clone(),
+        }
+    }
+}
+
+// keep the translation layer with py-sdk
+#[derive(Serialize)]
+pub struct LegacyExperiment {
+    id: u32,
+    name: String,
+    enabled: bool,
+    #[serde(rename = "type")]
+    feature_type: ExperimentType,
+    version: u32,
+    owner: String,
+    emit_event: bool,
+    value: Option<Value>,
+    value_type: Option<ValueType>,
+    targeting: Option<TargetingTree>,
+    overrides: Option<Vec<HashMap<String, TargetingTree>>>,
+    variant_set: Option<VariantSet>,
+}
+
+impl From<&Feature> for LegacyExperiment {
+    fn from(f: &Feature) -> Self {
+        let (feature_type, emit_event, value, value_type, targeting, overrides, variant_set) =
+            match f {
+                Feature::RangeVariant(rv) => (
+                    ExperimentType::RangeVariant,
+                    rv.emit_event,
+                    None,
+                    None,
+                    rv.targeting.clone(),
+                    rv.overrides.clone(),
+                    Some(rv.variant_set.clone()),
+                ),
+                Feature::DynamicConfig(dc) => (
+                    ExperimentType::DynamicConfig,
+                    false,
+                    Some(dc.value.clone()),
+                    Some(dc.value_type),
+                    None,
+                    None,
+                    None,
+                ),
+            };
+
+        LegacyExperiment {
+            id: f.metadata().id,
+            name: f.metadata().name.to_string(),
+            enabled: f.metadata().enabled,
+            version: f.metadata().version,
+            owner: f.metadata().owner.to_string(),
+            feature_type,
+            emit_event,
+            value,
+            value_type,
+            targeting,
+            overrides,
+            variant_set,
         }
     }
 }
 
+type FeatureName = String;
+
 /// Decider determines feature availability by chaining together simple decision maker
 /// functions to enable complicated logic to be expressed as a composition of simple,
 /// testable functions. Those compositions are tested against features, an abstraction
 /// for bits of code that enabling feature flagging, AB testing, etc..
 pub struct Decider {
-    features: Vec<Feature>,
+    features: HashMap<FeatureName, Feature>,
     decisionmakers: Vec<Decisionmaker>,
 }
 
 impl fmt::Debug for Decider {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         write!(f, "Decider: {:#?}", self.features)
     }
 }
 
 impl Decider {
+    const DEFAULT_DECISIONMAKERS: &'static str =
+        "darkmode overrides targeting holdout mutex_group fractional_availability value";
+
+    /// Creates a new `Decider` with the default decisionmakers. The experiment config is loaded
+    /// from the provided file path.
+    pub fn new(path: impl AsRef<Path>) -> Result<Self, DeciderInitError> {
+        let file = File::open(path)?;
+        let read = BufReader::new(file);
+
+        Self::from_bytes(read)
+    }
+
+    /// Creates a new `Decider` with the default decisionmakers. The experiment config is loaded
+    /// from the provided [`std::io::Read`].
+    pub fn from_bytes(config: impl Read) -> Result<Self, DeciderInitError> {
+        let value = serde_json::from_reader(config)?;
+
+        Self::with_decisionmakers(value, Self::DEFAULT_DECISIONMAKERS)
+    }
+
+    /// Creates a new `Decider` with an experiment config and a decisionmaker config string. Prefer
+    /// the other constructors for this type: customizing the set of decisionmakers is rarely what
+    /// you want.
+    pub fn with_decisionmakers(
+        config: Value,
+        decisionmakers: &str,
+    ) -> Result<Self, DeciderInitError> {
+        let raw_config: RawConfig = serde_json::from_value(config)?;
+        let (features, errs) = raw_config.features();
+
+        string_to_decisionmakers(decisionmakers).and_then(|decisionmakers| {
+            let decider = Decider {
+                features: features.into_iter().fold(HashMap::new(), |mut acc, f| {
+                    acc.insert(f.metadata().name.clone(), f);
+                    acc
+                }),
+                decisionmakers,
+            };
+
+            if errs.is_empty() {
+                Ok(decider)
+            } else {
+                Err(DeciderInitError::PartialLoad(decider, errs))
+            }
+        })
+    }
+
     pub fn choose(
         &self,
         feature_name: &str,
         ctx: &Context,
-        bucket_val_opt: Option<BucketVal>,
-    ) -> Result<Option<Decision>, DeciderError> {
+        bucketing_field_opt: Option<ContextField>,
+    ) -> Result<Decision, DeciderError> {
         let f = self.feature_by_name(feature_name)?;
-        match bucket_val_opt {
-            None => self.decide(f, ctx),
-            Some(bv) => match &f.variant_set {
-                None => Err(DeciderError::InvalidFeature),
-                Some(vs) => match &vs.bucket_val {
-                    Some(f_bv) => {
-                        if bv == *f_bv {
-                            self.decide(f, ctx)
-                        } else {
-                            Err(DeciderError::IdentifierTypeBucketValMismatch(
-                                bv.to_string(),
-                                f_bv.to_string(),
-                            ))
-                        }
+        if let Some(cf) = bucketing_field_opt {
+            match f {
+                Feature::RangeVariant(choice) => {
+                    if cf != choice.variant_set.bucketing_field {
+                        return Err(DeciderError::IdentifierTypeBucketValMismatch(
+                            cf,
+                            choice.variant_set.bucketing_field.clone(),
+                        ));
                     }
-                    None => Err(DeciderError::InvalidFeature),
-                },
-            },
+                }
+                Feature::DynamicConfig(_) => return Err(DeciderError::InvalidFeature),
+            }
         }
+
+        self.decide(f, ctx)
     }
 
     pub fn choose_all(
         &self,
         ctx: &Context,
-        bucket_val_opt: Option<BucketVal>,
-    ) -> Result<HashMap<String, Result<Option<Decision>, DeciderError>>, DeciderError> {
-        // FIXME: set this up such that we can filter by bucketing platform
-        match bucket_val_opt {
-            None => Ok(self
-                .features
-                .iter()
-                .filter_map(|f| match &f.feature_type {
-                    ExperimentType::DynamicConfig => None,
-                    _ => Some((f.name.clone(), self.decide(f, ctx))),
-                })
-                .collect()),
-            Some(bv) => Ok(self
-                .features
-                .iter()
-                .filter_map(|f| match &f.feature_type {
-                    ExperimentType::DynamicConfig => None,
-                    _ => match &f.variant_set {
-                        None => None,
-                        Some(vs) => match &vs.bucket_val {
-                            Some(f_bv) => {
-                                if bv == *f_bv {
-                                    Some((f.name.clone(), self.decide(f, ctx)))
-                                } else {
-                                    None
-                                }
-                            }
-                            None => None,
-                        },
-                    },
-                })
-                .collect()),
-        }
-    }
-
-    pub fn choose_for(
-        &self,
-        feature_name: &str,
-        s: String,
-        ctxo: &Option<Context>,
-    ) -> Result<Option<Decision>, DeciderError> {
-        let f = self.feature_by_name(feature_name)?;
-        match (ctxo, f.variant_set.clone()) {
-            (Some(ctx), None) => self.decide(f, ctx),
-            (Some(ctx), Some(vs)) => match &vs.bucket_val {
-                Some(bv) => {
-                    let ctxn = ctx.with_bucket_val(bv, s);
-                    self.decide(f, &ctxn)
+        bucketing_field_opt: Option<ContextField>,
+    ) -> HashMap<String, Result<Decision, DeciderError>> {
+        let cfo = bucketing_field_opt.as_ref();
+        self.features
+            .iter()
+            .fold(HashMap::new(), |mut acc, (name, f)| {
+                if let Feature::RangeVariant(rv) = f {
+                    // filter when the `bucketing_field_opt` is set, but return everything when it's `None`.
+                    if cfo.is_none() || Some(&rv.variant_set.bucketing_field) == cfo {
+                        acc.insert(name.to_string(), self.decide(f, ctx));
+                    }
                 }
-                None => Err(DeciderError::InvalidFeature),
-            },
-            (None, Some(vs)) => match &vs.bucket_val {
-                Some(bv) => self.decide(f, &Context::for_bucket_val(bv, s)),
-                None => Err(DeciderError::InvalidFeature),
-            },
-            (None, None) => Err(DeciderError::InvalidFeature),
-        }
+                acc
+            })
     }
 
     pub fn get_bool(&self, feature_name: &str, ctx: &Context) -> Result<bool, DeciderError> {
         match self.get_value(feature_name, ctx) {
             Ok(Value::Bool(b)) => Ok(b),
             Ok(_) => Err(DeciderError::DcTypeMismatch),
             Err(e) => Err(e),
@@ -566,419 +622,324 @@
             Ok(Value::Object(obj)) => Ok(obj),
             Ok(_) => Err(DeciderError::DcTypeMismatch),
             Err(e) => Err(e),
         }
     }
 
     pub fn get_all_values(&self, ctx: &Context) -> Result<HashMap<String, Decision>, DeciderError> {
-        Ok(self
-            .features
-            .iter()
-            .filter_map(|f| match &f.feature_type {
-                ExperimentType::DynamicConfig => Some((
-                    f.name.clone(),
-                    match self.decide(f, ctx) {
-                        Ok(Some(decision)) => decision,
-                        _ => Decision {
-                            feature_id: f.id,
-                            feature_name: f.name.clone(),
-                            feature_version: f.version,
-                            variant_name: None,
-                            value: set_default_value(f.value_type.as_ref()),
-                            value_type: f.value_type.clone(),
-                            event_data: vec![],
-                            events: vec![],
-                        },
-                    },
-                )),
-                _ => None,
-            })
-            .collect())
+        Ok(self.features.values().fold(HashMap::new(), |mut acc, f| {
+            if let Feature::DynamicConfig(dc) = f {
+                let decision = self.decide(f, ctx).unwrap_or(Decision {
+                    feature_id: dc.metadata.id,
+                    feature_name: dc.metadata.name.clone(),
+                    feature_version: dc.metadata.version,
+                    variant_name: None,
+                    value: dc.value.clone(),
+                    value_type: Some(dc.value_type),
+                    event_data: vec![],
+                    events: vec![],
+                });
+                acc.insert(f.metadata().name.clone(), decision);
+            }
+            acc
+        }))
     }
 
     pub fn feature_by_name(&self, feature_name: &str) -> Result<&Feature, DeciderError> {
-        match self.features.iter().find(|f| f.name == feature_name) {
+        match self.features.get(feature_name) {
+            Some(feature) => Ok(feature),
             None => Err(DeciderError::FeatureNotFoundWithName(
                 feature_name.to_string(),
             )),
-            Some(feature) => Ok(feature),
         }
     }
 
     fn get_value(&self, feature_name: &str, ctx: &Context) -> Result<Value, DeciderError> {
         let f = self.feature_by_name(feature_name)?;
         match self.decide(f, ctx) {
             Err(e) => Err(e),
-            Ok(None) => Err(DeciderError::InvalidFeature),
-            Ok(Some(Decision { value, .. })) => Ok(value),
+            Ok(Decision { value, .. }) => Ok(value),
         }
     }
 
-    fn decide(&self, f: &Feature, ctx: &Context) -> Result<Option<Decision>, DeciderError> {
+    fn decide(&self, f: &Feature, ctx: &Context) -> Result<Decision, DeciderError> {
         // First, call `decide_internal` to get an `InternalDecision`...
-        self.decide_internal(f, ctx).and_then(|io| {
+        self.decide_internal(f, ctx).and_then(|internal| {
             // If that succeeded, hydrate the event strings and convert to a `Decision`.
-            io.map(|internal| {
-                let serialized_events = SerializedEvents::new(ctx, internal.events)
-                    .map_err(DeciderError::MalformedEventError)?;
-
-                Ok(Decision {
-                    feature_id: internal.feature_id,
-                    feature_name: internal.feature_name,
-                    feature_version: internal.feature_version,
-                    variant_name: internal.variant_name,
-                    value: internal.value,
-                    value_type: internal.value_type,
-                    event_data: serialized_events.event_data,
-                    events: serialized_events.events,
-                })
+
+            let serialized_events = SerializedEvents::new(ctx, internal.events)
+                .map_err(DeciderError::MalformedEventError)?;
+
+            Ok(Decision {
+                feature_id: internal.feature_id,
+                feature_name: internal.feature_name,
+                feature_version: internal.feature_version,
+                variant_name: internal.variant_name,
+                value: internal.value,
+                value_type: internal.value_type,
+                event_data: serialized_events.event_data,
+                events: serialized_events.events,
             })
-            .transpose()
         })
     }
 
     fn decide_internal(
         &self,
-        f: &Feature,
+        feature: &Feature,
         ctx: &Context,
-    ) -> Result<Option<InternalDecision>, DeciderError> {
-        // TODO: decide whether decide should return a Result<Option<Decision>>, to
-        //       account for ill-defined Features or missing data on the Context. Probably
-        //       yes, but currently Decision also has an option on name/bucketing.  Maybe
-        //       decide should return a Result<Decision>?
+    ) -> Result<InternalDecision, DeciderError> {
         let mut out = vec![];
         for fun in &self.decisionmakers {
-            match fun(self, f, ctx)? {
-                Choice::None => return Ok(None),
+            match fun(self, feature, ctx)? {
+                Choice::None => break,
                 Choice::Pass(_) => (),
                 Choice::Continue(events) => out.extend(events),
-                Choice::Decided(mut d) => {
+                Choice::Decided(mut decision) => {
                     if !out.is_empty() {
-                        out.extend(d.events);
-                        d.events = out;
+                        out.extend(decision.events);
+                        decision.events = out;
                     }
-                    return Ok(Some(d));
+                    return Ok(decision);
                 }
             }
         }
-        Ok(None)
+        // If we make it here that means a decision couldn't be made, either because no
+        // decisionmaker returned `Choice::Decided`, or because a decisionmaker short-circuited via
+        // `Choice::None`. Return a default decision to preserve events.
+        Ok(feature.default_decision(out))
     }
 
     fn holdout(&self, f: &Feature, ctx: &Context) -> Result<Choice, DeciderError> {
-        let hgo = f.variant_set.as_ref().and_then(|vs| vs.holdout.as_ref());
-        match hgo {
-            None => Ok(Choice::Pass("no_holdout_group")),
-            Some(hg) => match self.decide_internal(hg, ctx) {
-                Err(e) => Err(e),
-                Ok(None) => Ok(Choice::Pass("in_holdout:false")),
-                Ok(Some(d)) => match d.variant_name {
-                    None => Ok(Choice::Pass("in_holdout:false")),
-                    Some(s) => {
-                        let mut events = d.events;
-                        DecisionKind::Holdout.cast_events(&mut events);
-
-                        match s.as_str() {
-                            "control_1" => Ok(Choice::Continue(events)),
-                            "holdout" => Ok(Choice::Decided(InternalDecision {
-                                feature_id: f.id,
-                                feature_name: f.name.to_string(),
-                                feature_version: f.version,
-                                variant_name: None,
-                                value: hg.value.clone().unwrap_or_default(),
-                                value_type: hg.value_type.clone(),
-                                events,
-                            })),
-                            _ => Ok(Choice::Pass("in_holdout:false")),
-                        }
-                    }
-                },
-            },
-        }
+        f.holdout(self, ctx)
     }
 
     fn mutex_group(&self, f: &Feature, ctx: &Context) -> Result<Choice, DeciderError> {
-        let mgo = &f
-            .variant_set
-            .as_ref()
-            .and_then(|vs| vs.mutex_group.as_ref());
-        match mgo {
-            None => Ok(Choice::Pass("no_mutex_group")),
-            Some(mg) => match self.decide_internal(mg, ctx) {
-                Err(e) => Err(e),
-                Ok(None) => Ok(Choice::None), // I'm not in the mutex group exp.
-                Ok(Some(InternalDecision {
-                    variant_name: Some(s),
-                    mut events,
-                    ..
-                })) => {
-                    // I got a decision!  But am I in the experiment I was asked for?
-                    if s == f.name {
-                        // Yes.  yes I am.  Let control flow through to the experiments
-                        DecisionKind::MutexGroup.cast_events(&mut events);
-                        Ok(Choice::Continue(events))
-                    } else {
-                        // not in exp, terminate early.
-                        Ok(Choice::None)
-                    }
-                }
-                _ => Ok(Choice::None),
-            },
-        }
-    }
-
-    fn darkmode(&self, f: &Feature, _ctx: &Context) -> Result<Choice, DeciderError> {
-        if f.enabled {
-            Ok(Choice::Pass("darkmode:enabled"))
-        } else {
-            Ok(Choice::None)
-        }
+        f.mutex_group(self, ctx)
     }
 
-    fn locale(&self, f: &Feature, _ctx: &Context) -> Result<Choice, DeciderError> {
-        if !f.enabled {
-            // TODO: add locales to Feature, compare ctx.locale to that
-            Ok(Choice::Pass("locale:fixme"))
-        } else {
-            Ok(Choice::Pass("locale:fixme2"))
-        }
+    fn darkmode(&self, f: &Feature, ctx: &Context) -> Result<Choice, DeciderError> {
+        f.darkmode(self, ctx)
     }
 
     fn fractional_availability(&self, f: &Feature, ctx: &Context) -> Result<Choice, DeciderError> {
-        match &f.variant_set {
-            None => Ok(Choice::Pass("frac_avail:no variant_set")),
-            Some(vs) => vs.get_bucket(f, ctx),
-        }
+        f.fractional_availability(self, ctx)
     }
 
     fn overrides(&self, f: &Feature, ctx: &Context) -> Result<Choice, DeciderError> {
-        match &f.overrides {
-            None => Ok(Choice::Pass("overrides:none_found")),
-            Some(ov) => {
-                for hm in ov.iter() {
-                    for (name, tt) in hm.iter() {
-                        match tt.eval(ctx) {
-                            Err(_) => {
-                                // FIXME: propagate the error and continue
-                                return Ok(Choice::Pass("t.eval:err"));
-                            }
-                            Ok(true) => {
-                                let event = f.make_event(DecisionKind::Override, name, ctx)?;
-
-                                return Ok(Choice::Decided(InternalDecision {
-                                    feature_id: f.id,
-                                    feature_name: f.name.to_string(),
-                                    feature_version: f.version,
-                                    // FIXME: check to make sure this is a variant name
-                                    variant_name: Some(name.clone()),
-                                    value: Value::String(name.clone()),
-                                    value_type: Some(ValueType::String),
-                                    events: Vec::from_iter(event),
-                                }));
-                            }
-                            Ok(false) => continue,
-                        }
-                    }
-                }
-                Ok(Choice::Pass("overrides:none_hit"))
-            }
-        }
+        f.overrides(self, ctx)
     }
 
     fn targeting(&self, f: &Feature, ctx: &Context) -> Result<Choice, DeciderError> {
-        match &f.targeting {
-            None => Ok(Choice::Pass("targeting:none_found")),
-            Some(tt) => match tt.eval(ctx) {
-                Err(_) => Ok(Choice::None), // FIXME: propagate the error
-                Ok(true) => Ok(Choice::Pass("targeting:targeted")),
-                Ok(false) => Ok(Choice::None),
-            },
-        }
+        f.targeting(self, ctx)
     }
 
-    fn value(&self, f: &Feature, _ctx: &Context) -> Result<Choice, DeciderError> {
-        match &f.value {
-            None => Ok(Choice::None),
-            Some(value) => match value {
-                Value::Null | Value::Array(_) => Ok(Choice::Pass("value:null_or_array")),
-                _ => Ok(Choice::Decided(InternalDecision {
-                    feature_id: f.id,
-                    feature_name: f.name.to_string(),
-                    feature_version: f.version,
-                    variant_name: None,
-                    value: value.clone(),
-                    value_type: f.value_type.clone(),
-                    events: vec![],
-                })),
-            },
-        }
+    fn value(&self, f: &Feature, ctx: &Context) -> Result<Choice, DeciderError> {
+        f.value(self, ctx)
     }
 }
 
+/// Variants are primarily used for fractional availability, where, eg., 10% of users
+/// are exposed to a given version of a feature.
+#[derive(Serialize, Deserialize, Debug, Clone, PartialEq, Eq)]
+pub struct Variant {
+    pub name: String,
+    #[serde(with = "variant_range_aux", flatten)]
+    pub range: Range<u16>,
+}
+
+const TOTAL_BUCKETS: u16 = 1000;
+
+/// The sentinel value for the "no variant override" variant.
+static NO_VARIANT_OVERRIDE: &str = "$none";
+
+mod variant_range_aux {
+    use crate::TOTAL_BUCKETS;
+    use serde::{Deserialize, Deserializer, Serialize, Serializer};
+    use std::ops::Range;
+
+    #[derive(Serialize, Deserialize)]
+    struct FloatRangeProxy {
+        range_start: f32,
+        range_end: f32,
+    }
+
+    /// Serializes a `Range<u16>` into a floating-point range using `FloatRangeProxy`.
+    /// `TOTAL_BUCKETS` is used as the upper limit of the range.
+    ///
+    /// Expects the input range to have 0.0 <= start <= 1.0 and 0.0 <= end <= 1.0.
+    pub fn serialize<S>(range: &Range<u16>, ser: S) -> Result<S::Ok, S::Error>
+    where
+        S: Serializer,
+    {
+        let proxy = FloatRangeProxy {
+            range_start: (range.start as f32) / (TOTAL_BUCKETS as f32),
+            range_end: (range.end as f32) / (TOTAL_BUCKETS as f32),
+        };
+
+        proxy.serialize(ser)
+    }
+
+    /// Deserializes a `Range<u16>` from a floating-point range using `FloatRangeProxy`.
+    /// `TOTAL_BUCKETS` is used as the upper limit of the range.
+    ///
+    /// The resulting range is guaranteed to have 0 <= start <= TOTAL_BUCKETS and
+    /// 0 <= end <= TOTAL_BUCKETS.
+    pub fn deserialize<'de, D>(des: D) -> Result<Range<u16>, D::Error>
+    where
+        D: Deserializer<'de>,
+    {
+        let proxy = FloatRangeProxy::deserialize(des)?;
+        let range = Range {
+            start: (proxy.range_start * (TOTAL_BUCKETS as f32)).floor() as u16,
+            end: (proxy.range_end * (TOTAL_BUCKETS as f32)).floor() as u16,
+        };
+
+        Ok(range)
+    }
+}
+
+/// VariantSet contains an experiment's variants, and all other fields not in common
+/// with dynamic config json.
+#[derive(Serialize, Deserialize, Debug, Clone)]
+pub struct VariantSet {
+    pub start_ts: u64, // TODO: consider whether this should just be created_at
+    pub stop_ts: u64,  // TODO: should we get rid of a version by creating a new one?
+    pub shuffle_version: u32,
+    #[serde(rename = "bucket_val")]
+    pub bucketing_field: ContextField,
+    variants: Vec<Variant>,
+    holdout: Option<Box<Feature>>,
+    mutex_group: Option<Box<Feature>>,
+}
+
 impl VariantSet {
-    fn bucketing_string(&self, exp_id: &u32, name: &str, identifier: &str) -> String {
+    fn bucketing_string(&self, exp_id: &u32, name: &str, bucket_val: Value) -> String {
+        let identifier = match bucket_val {
+            // Json strings are formatted surrounded by quotes. Extract the inner value
+            // to avoid this.
+            Value::String(inner) => inner,
+            _ => bucket_val.to_string(),
+        };
+
         format!("{}.{}.{}{}", exp_id, name, self.shuffle_version, identifier)
     }
 
-    fn get_bucket(&self, f: &Feature, ctx: &Context) -> Result<Choice, DeciderError> {
-        let identifier = ctx.get_bucketing_field(self.bucket_val.as_ref())?;
-        let bucketing_string = self.bucketing_string(&f.id, &f.name, &identifier);
-        let i = bucket(&bucketing_string)?;
-        let flt = (i as f32) / 1000.0;
-        let v = self.variants.iter().find(|x| x.lo <= flt && x.hi > flt);
+    fn get_bucket(&self, f: &RangeVariant, ctx: &Context) -> Result<Choice, DeciderError> {
+        let identifier = self.bucketing_field.get_value(ctx).ok_or_else(|| {
+            DeciderError::MissingBucketingFieldInContext(self.bucketing_field.clone())
+        })?;
+
+        let bucketing_string = self.bucketing_string(&f.metadata.id, &f.metadata.name, identifier);
+        let bucket = self.bucket_from_str(&bucketing_string);
+        let v = self.variants.iter().find(|x| x.range.contains(&bucket));
         match v {
             None => Ok(Choice::Pass("frac_avail:not in variants")),
             Some(variant) => Ok(Choice::Decided(InternalDecision {
-                feature_id: f.id,
-                feature_name: f.name.to_string(),
-                feature_version: f.version,
+                feature_id: f.metadata.id,
+                feature_name: f.metadata.name.to_string(),
+                feature_version: f.metadata.version,
                 variant_name: Some(variant.name.clone()),
                 value: Value::Null,
                 value_type: None,
                 events: Vec::from_iter(f.make_event(
                     DecisionKind::FracAvail,
                     &variant.name,
                     ctx,
                 )?),
             })),
         }
     }
+
+    fn bucket_from_str(&self, bucketing_str: &str) -> u16 {
+        // FIXME: take in number of buckets as a param.
+        let mut hasher = Sha1::new();
+        hasher.update(bucketing_str);
+        let bigint = BigUint::from_bytes_be(hasher.finalize().as_ref());
+
+        u16::try_from(bigint % TOTAL_BUCKETS)
+            .expect("bigint has max value of 1000, should fit in a u16")
+    }
 }
 
 #[derive(Debug)]
 enum Choice {
     // TODO: find a better nome
     Pass(&'static str),             // I didn't make a decision because...
     None,                           // response is nothing
     Continue(Vec<ExperimentEvent>), // a parent decision got called, so save its events and continue
     Decided(InternalDecision),      // an actual decision.
 }
 
-#[derive(Debug)]
+#[derive(Debug, Error)]
 pub enum DeciderError {
-    FeatureNotFound,
+    #[error("Feature \"{0}\" not found")]
     FeatureNotFoundWithName(String),
+    #[error("Invalid feature configuration")]
     InvalidFeature,
+    #[error("Missing \"bucket_val\" field in experiment config")]
     MissingBucketVal,
-    MissingBucketValInContext(String),
-    IdentifierTypeBucketValMismatch(String, String),
-    IncorrectBucketValString(String),
-    BucketingError(String),
+    #[error("Missing field \"{0}\" in context for bucket_val = {0}")]
+    MissingBucketingFieldInContext(ContextField),
+    #[error(
+        "Requested identifier_type \"{0}\" is incompatible with experiment's bucket_val = {1}"
+    )]
+    IdentifierTypeBucketValMismatch(ContextField, ContextField),
+    #[error("Missing variant_set")]
     MissingVariantSet,
+    #[error("Dynamic Configuration Feature type mismatch")]
     DcTypeMismatch,
+    #[error("Number deserialization failed")]
     NumberDeserializationError,
-    MapDeserializationError(String),
-    MalformedEventError(Box<dyn Error>),
+    #[error("Decider returned malformed event: {0}")]
+    MalformedEventError(#[source] Box<dyn Error>),
 }
 
-impl Error for DeciderError {}
-
-impl fmt::Display for DeciderError {
-    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        match &*self {
-            DeciderError::FeatureNotFound => write!(f, "Feature not found."),
-            DeciderError::FeatureNotFoundWithName(name) => {
-                write!(f, "Feature {:#?} not found.", name)
-            }
-            DeciderError::InvalidFeature => write!(f, "Invalid Feature configuration."),
-            DeciderError::BucketingError(s) => write!(f, "{}", s),
-            DeciderError::MissingBucketVal => {
-                write!(f, "Missing \"bucket_val\" field in experiment config.")
-            }
-            DeciderError::MissingBucketValInContext(bucket_val) => write!(
-                f,
-                "Missing {:#?} in context for bucket_val = {:#?}",
-                bucket_val, bucket_val
-            ),
-            DeciderError::IdentifierTypeBucketValMismatch(bucket_val_string, feature_bucket_val) => write!(
-                f,
-                "Requested identifier_type: {:#?} is incompatible with experiment's \"bucket_val\" = {:#?}.",
-                bucket_val_string, feature_bucket_val
-            ),
-            DeciderError::IncorrectBucketValString(bvs) => write!(
-                f,
-                "identifier_type: {:#?} is not a supported \"bucket_val\".",
-                bvs
-            ),
-            DeciderError::MissingVariantSet => write!(f, "Missing variant_set"),
-            DeciderError::DcTypeMismatch => {
-                write!(f, "Dynamic Configuration Feature type mismatch.")
-            }
-            DeciderError::NumberDeserializationError => {
-                write!(f, "Number deserialization failed.")
-            }
-            DeciderError::MapDeserializationError(err_str) => {
-                write!(f, "Map deserialization failed: {:#?}", err_str)
-            }
-            DeciderError::MalformedEventError(inner) => write!(f, "Decider returned malformed event: {}", inner),
-        }
-    }
-}
-
-#[derive(Debug)]
+#[derive(Debug, Error)]
 pub enum DeciderInitError {
-    IoError(std::io::Error),
-    SerdeError(serde_json::Error),
+    #[error("Std io error: {0}")]
+    IoError(
+        #[from]
+        #[source]
+        std::io::Error,
+    ),
+    #[error("Json error: {0}")]
+    SerdeError(
+        #[from]
+        #[source]
+        serde_json::Error,
+    ),
+    #[error("Invalid decisionmaker: {0:?}")]
     InvalidDecisionMaker(String),
-}
-
-impl Error for DeciderInitError {
-    fn source(&self) -> Option<&(dyn Error + 'static)> {
-        match self {
-            Self::IoError(src) => Some(src),
-            Self::SerdeError(src) => Some(src),
-            _ => None,
-        }
-    }
-}
-
-impl fmt::Display for DeciderInitError {
-    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        match &*self {
-            DeciderInitError::InvalidDecisionMaker(err_str) => {
-                write!(f, "Invalid DecisionMaker: {:#?}", err_str.clone())
-            }
-            DeciderInitError::SerdeError(serde_json_error) => {
-                write!(f, "Json error: {:#?}", serde_json_error.to_string())
-            }
-            DeciderInitError::IoError(std_io_error) => {
-                write!(f, "Std io error: {:#?}", std_io_error.to_string())
-            }
-        }
-    }
-}
-
-impl From<std::io::Error> for DeciderInitError {
-    fn from(e: std::io::Error) -> DeciderInitError {
-        DeciderInitError::IoError(e)
-    }
-}
-
-impl From<serde_json::Error> for DeciderInitError {
-    fn from(e: serde_json::Error) -> DeciderInitError {
-        DeciderInitError::SerdeError(e)
-    }
+    #[error("Partially loaded Decider: {} features failed to load", .1.len())]
+    PartialLoad(Decider, HashMap<String, serde_json::Error>),
 }
 
 /// An `Event` holds a hydrated exposure event, serialized as a json string, as well as an explicit
 /// `DecisionKind`. The kind can be used by the client to choose whether to expose this event.
-#[derive(Debug, Clone, PartialEq, Eq)]
+#[derive(Serialize, Debug, Clone, PartialEq, Eq)]
 pub struct Event {
     pub kind: DecisionKind,
+
+    /// A unique key for this exposure. Equivalent exposures will have the same exposure key.
+    /// Clients may use this key to keep track of events that were exposed previously.
+    pub exposure_key: String,
+
     pub json: String,
 }
 
-#[derive(Debug, Clone, PartialEq, Eq)]
+#[derive(Serialize, Debug, Clone, PartialEq, Eq)]
 pub struct Decision {
     pub feature_id: u32,
     pub feature_name: String,
     pub feature_version: u32,
     pub variant_name: Option<String>,
     pub value: Value,
     pub value_type: Option<ValueType>,
     // TODO Remove event_data once we've migrated off of the legacy string format.
+    #[serde(skip)]
     pub event_data: Vec<String>,
     pub events: Vec<Event>,
 }
 
 /// An `InternalDecision` holds the same data as a [Decision] except contains a list of
 /// [ExperimentEvent] instead of hydrated strings. It's returned from the [Decisionmaker]s and
 /// internal decider methods, and is converted to a `Decision` before returning from `decide`.
@@ -989,85 +950,354 @@
     feature_version: u32,
     variant_name: Option<String>,
     value: Value,
     value_type: Option<ValueType>,
     events: Vec<ExperimentEvent>,
 }
 
-fn bucket(bucketing_str: &str) -> Result<i32, DeciderError> {
-    // FIXME: take in number of buckets as a param.
-    let mut hasher = Sha1::new();
-    hasher.input_str(bucketing_str);
-    let bigint_opt = BigUint::parse_bytes(hasher.result_str().as_bytes(), 16);
-    let bigint_res = match bigint_opt {
-        Some(v) => Ok(v % 1000u32),
-        None => Err(DeciderError::BucketingError(format!(
-            "'{}' failed",
-            bucketing_str
-        ))),
-    };
-    match i32::try_from(bigint_res?) {
-        Ok(i) => Ok(i),
-        Err(_) => Err(DeciderError::BucketingError("bigint fail".to_string())),
+trait Decide {
+    fn darkmode(&self, d: &Decider, ctx: &Context) -> Result<Choice, DeciderError>;
+    fn fractional_availability(&self, d: &Decider, ctx: &Context) -> Result<Choice, DeciderError>;
+    fn targeting(&self, d: &Decider, ctx: &Context) -> Result<Choice, DeciderError>;
+    fn overrides(&self, d: &Decider, ctx: &Context) -> Result<Choice, DeciderError>;
+    fn value(&self, d: &Decider, ctx: &Context) -> Result<Choice, DeciderError>;
+    fn holdout(&self, d: &Decider, ctx: &Context) -> Result<Choice, DeciderError>;
+    fn mutex_group(&self, d: &Decider, ctx: &Context) -> Result<Choice, DeciderError>;
+}
+
+impl Decide for Feature {
+    fn darkmode(&self, d: &Decider, ctx: &Context) -> Result<Choice, DeciderError> {
+        match self {
+            Feature::RangeVariant(rv) => rv.darkmode(d, ctx),
+            Feature::DynamicConfig(dc) => dc.darkmode(d, ctx),
+        }
+    }
+
+    fn fractional_availability(&self, d: &Decider, ctx: &Context) -> Result<Choice, DeciderError> {
+        match self {
+            Feature::RangeVariant(rv) => rv.fractional_availability(d, ctx),
+            Feature::DynamicConfig(dc) => dc.fractional_availability(d, ctx),
+        }
+    }
+
+    fn targeting(&self, d: &Decider, ctx: &Context) -> Result<Choice, DeciderError> {
+        match self {
+            Feature::RangeVariant(rv) => rv.targeting(d, ctx),
+            Feature::DynamicConfig(dc) => dc.targeting(d, ctx),
+        }
+    }
+
+    fn overrides(&self, d: &Decider, ctx: &Context) -> Result<Choice, DeciderError> {
+        match self {
+            Feature::RangeVariant(rv) => rv.overrides(d, ctx),
+            Feature::DynamicConfig(dc) => dc.overrides(d, ctx),
+        }
+    }
+
+    fn value(&self, d: &Decider, ctx: &Context) -> Result<Choice, DeciderError> {
+        match self {
+            Feature::RangeVariant(rv) => rv.value(d, ctx),
+            Feature::DynamicConfig(dc) => dc.value(d, ctx),
+        }
+    }
+
+    fn holdout(&self, d: &Decider, ctx: &Context) -> Result<Choice, DeciderError> {
+        match self {
+            Feature::RangeVariant(rv) => rv.holdout(d, ctx),
+            Feature::DynamicConfig(dc) => dc.holdout(d, ctx),
+        }
+    }
+
+    fn mutex_group(&self, d: &Decider, ctx: &Context) -> Result<Choice, DeciderError> {
+        match self {
+            Feature::RangeVariant(rv) => rv.mutex_group(d, ctx),
+            Feature::DynamicConfig(dc) => dc.mutex_group(d, ctx),
+        }
+    }
+}
+
+impl Decide for RangeVariant {
+    fn darkmode(&self, _d: &Decider, _ctx: &Context) -> Result<Choice, DeciderError> {
+        if self.enabled {
+            Ok(Choice::Pass("darkmode:enabled"))
+        } else {
+            Ok(Choice::None)
+        }
+    }
+
+    fn fractional_availability(&self, _d: &Decider, ctx: &Context) -> Result<Choice, DeciderError> {
+        self.variant_set.get_bucket(self, ctx)
+    }
+
+    fn targeting(&self, _d: &Decider, ctx: &Context) -> Result<Choice, DeciderError> {
+        match &self.targeting {
+            None => Ok(Choice::Pass("targeting:none_found")),
+            Some(tt) => match tt.eval(ctx) {
+                Some(true) => Ok(Choice::Pass("targeting:targeted")),
+                Some(false) => Ok(Choice::None),
+                None => Ok(Choice::None), // FIXME: propagate the error
+            },
+        }
+    }
+
+    fn overrides(&self, _d: &Decider, ctx: &Context) -> Result<Choice, DeciderError> {
+        let decicion_for_override = |name: &String| -> Result<Choice, DeciderError> {
+            let variant_name = if name != NO_VARIANT_OVERRIDE {
+                Some(name.clone())
+            } else {
+                None
+            };
+
+            if variant_name.is_some()
+                && !self.variant_set.variants.iter().any(|v| &v.name == name)
+            {
+                return Ok(Choice::Pass("overrides:variant_not_found"));
+            }
+
+            Ok(Choice::Decided(InternalDecision {
+                feature_id: self.metadata.id,
+                feature_name: self.metadata.name.to_string(),
+                feature_version: self.metadata.version,
+                variant_name,
+                value: Value::Null,
+                value_type: None,
+                events: Vec::from_iter(self.make_event(DecisionKind::Override, name, ctx)?),
+            }))
+        };
+
+        match &self.overrides {
+            None => Ok(Choice::Pass("overrides:none_found")),
+            Some(ov) => {
+                for hm in ov.iter() {
+                    for (name, tt) in hm.iter() {
+                        match tt.eval(ctx) {
+                            Some(true) => {
+                                return decicion_for_override(name);
+                            }
+                            Some(false) => continue,
+                            None => {
+                                // FIXME: propagate the error and continue
+                                return Ok(Choice::Pass("t.eval:err"));
+                            }
+                        }
+                    }
+                }
+                Ok(Choice::Pass("overrides:none_hit"))
+            }
+        }
+    }
+
+    fn value(&self, _d: &Decider, _ctx: &Context) -> Result<Choice, DeciderError> {
+        Ok(Choice::None)
+    }
+
+    fn holdout(&self, d: &Decider, ctx: &Context) -> Result<Choice, DeciderError> {
+        match self.variant_set.holdout.as_ref() {
+            None => Ok(Choice::Pass("no_holdout_group")),
+            Some(hg) => d
+                .decide_internal(hg, ctx)
+                .map(|result| match result.variant_name {
+                    None => Choice::Pass("in_holdout:false"),
+                    Some(s) => {
+                        let mut events = result.events;
+                        DecisionKind::Holdout.cast_events(&mut events);
+
+                        match s.as_str() {
+                            "control_1" => Choice::Continue(events),
+                            "holdout" => Choice::Decided(InternalDecision {
+                                feature_id: self.metadata.id,
+                                feature_name: self.metadata.name.to_string(),
+                                feature_version: self.metadata.version,
+                                variant_name: None,
+                                value: Value::Null,
+                                value_type: None,
+                                events,
+                            }),
+                            _ => Choice::Pass("in_holdout:false"),
+                        }
+                    }
+                }),
+        }
+    }
+
+    fn mutex_group(&self, d: &Decider, ctx: &Context) -> Result<Choice, DeciderError> {
+        match self.variant_set.mutex_group.as_ref() {
+            None => Ok(Choice::Pass("no_mutex_group")),
+            Some(mg) => match d.decide_internal(mg, ctx) {
+                Err(e) => Err(e),
+                Ok(InternalDecision {
+                    variant_name: Some(s),
+                    mut events,
+                    ..
+                }) => {
+                    // I got a decision!  But am I in the experiment I was asked for?
+                    if s == self.metadata.name {
+                        // Yes.  yes I am.  Let control flow through to the experiments
+                        DecisionKind::MutexGroup.cast_events(&mut events);
+                        Ok(Choice::Continue(events))
+                    } else {
+                        // not in exp, terminate early.
+                        Ok(Choice::None)
+                    }
+                }
+                // I'm not in the mutex group experiment.
+                _ => Ok(Choice::None),
+            },
+        }
+    }
+}
+
+impl Decide for DynamicConfig {
+    fn darkmode(&self, _d: &Decider, _ctx: &Context) -> Result<Choice, DeciderError> {
+        Ok(Choice::None)
+    }
+
+    fn fractional_availability(
+        &self,
+        _d: &Decider,
+        _ctx: &Context,
+    ) -> Result<Choice, DeciderError> {
+        Ok(Choice::Pass("frac_avail:no variant_set"))
+    }
+
+    fn targeting(&self, _d: &Decider, _ctx: &Context) -> Result<Choice, DeciderError> {
+        Ok(Choice::Pass("targeting:none_found"))
+    }
+
+    fn overrides(&self, _d: &Decider, _ctx: &Context) -> Result<Choice, DeciderError> {
+        Ok(Choice::Pass("overrides:none_found"))
+    }
+
+    fn value(&self, _d: &Decider, _ctx: &Context) -> Result<Choice, DeciderError> {
+        match self.value {
+            Value::Null | Value::Array(_) => Ok(Choice::Pass("value:null_or_array")),
+            _ => Ok(Choice::Decided(InternalDecision {
+                feature_id: self.metadata.id,
+                feature_name: self.metadata.name.to_string(),
+                feature_version: self.metadata.version,
+                variant_name: None,
+                value: self.value.clone(),
+                value_type: Some(self.value_type),
+                events: vec![],
+            })),
+        }
+    }
+
+    fn holdout(&self, _d: &Decider, _ctx: &Context) -> Result<Choice, DeciderError> {
+        Ok(Choice::Pass("no_holdout_group"))
+    }
+
+    fn mutex_group(&self, _d: &Decider, _ctx: &Context) -> Result<Choice, DeciderError> {
+        Ok(Choice::Pass("no_mutex_group"))
     }
 }
 
 type Decisionmaker = fn(d: &Decider, f: &Feature, ctx: &Context) -> Result<Choice, DeciderError>;
 
-fn name_to_decisionmaker(name: &str) -> Result<Decisionmaker, String> {
-    return match name {
+fn name_to_decisionmaker(name: &str) -> Result<Decisionmaker, DeciderInitError> {
+    match name {
         "darkmode" => Ok(Decider::darkmode),
-        "locale" => Ok(Decider::locale),
         "fractional_availability" => Ok(Decider::fractional_availability),
         "targeting" => Ok(Decider::targeting),
         "overrides" => Ok(Decider::overrides),
         "value" => Ok(Decider::value),
         "holdout" => Ok(Decider::holdout),
         "mutex_group" => Ok(Decider::mutex_group),
-        _ => Err(format!("Invalid decisionmaker name: {:?}", name)),
-    };
+        _ => Err(DeciderInitError::InvalidDecisionMaker(format!(
+            "Invalid decisionmaker name: {:?}",
+            name
+        ))),
+    }
 }
 
-fn string_to_decisionmakers(cfg: &str) -> Result<Vec<Decisionmaker>, String> {
+fn string_to_decisionmakers(cfg: &str) -> Result<Vec<Decisionmaker>, DeciderInitError> {
     // we get a result of a vec because we want any single error in
     // decisionmaker names to fail the whole thing (no silent errors
     // causing unexpected behavior).  Got the technique from:
     // https://stackoverflow.com/questions/26368288/how-do-i-stop-iteration-and-return-an-error-when-iteratormap-returns-a-result
     cfg.split_whitespace().map(name_to_decisionmaker).collect()
 }
 
-pub fn init(cfg: &str, features: Vec<Feature>) -> Result<Decider, DeciderInitError> {
-    match string_to_decisionmakers(cfg) {
-        Ok(decisionmakers) => Ok(Decider {
-            features,
-            decisionmakers,
-        }),
-        Err(s) => Err(DeciderInitError::InvalidDecisionMaker(s)),
-    }
-}
-
 // This section is legacy code to deal with reddit's existing experiment format.
-pub fn init_decider<P: AsRef<Path>>(cfg: &str, filepath: P) -> Result<Decider, DeciderInitError> {
+#[deprecated(note = "use Decider::new instead")]
+pub fn init_decider<P: AsRef<Path>>(
+    decisionmakers: &str,
+    filepath: P,
+) -> Result<Decider, DeciderInitError> {
     let file = File::open(filepath)?;
     let reader = BufReader::new(file);
-    let ec: ExperimentConfig = serde_json::from_reader(reader)?;
-    let fl = experiment_config_to_features(ec)?;
-    init(cfg, fl)
+    let config = serde_json::from_reader(reader)?;
+
+    Decider::with_decisionmakers(config, decisionmakers)
 }
 
-fn experiment_config_to_features(ec: ExperimentConfig) -> Result<Vec<Feature>, DeciderInitError> {
-    let ec2 = ec.clone();
-    let fl: Vec<Feature> = ec
-        .into_values()
-        .map(|exp| experiment_to_feature(&exp, &ec2))
-        .collect();
-    Ok(fl)
+struct ExperimentConfig {
+    experiments: HashMap<String, Experiment>,
+    override_groups: HashMap<String, OverrideGroup>,
 }
 
-type ExperimentConfig = HashMap<String, Experiment>;
+fn experiment_config_to_features(ec: &ExperimentConfig) -> Vec<Feature> {
+    ec.experiments
+        .values()
+        .map(|exp| experiment_to_feature(exp, ec))
+        .collect()
+}
+
+/// An intermediate struct representing a raw experiment config. The experiments are parsed as
+/// JSON values.
+///
+/// This struct allows us to partially load [`Decider`]. When deserializing into a specific type,
+/// serde will return an error if any part of the type can't be properly deserialized. This means
+/// that if we deserialize into a `HashMap<String, Experiment>`, and any key in the object is not a
+/// valid experiment, the entire object is invalid.
+///
+/// Any valid JSON can be deserialized into a [`Value`], though. When we deserialize the input into
+/// a [`RawConfig`], serde will check that:
+///   - The input is a valid JSON object.
+///   - Each key in the object maps to a valid JSON value.
+///
+/// We can then individually deserialize the [`Value`]s into [`Feature`]s, and partially load a
+/// decider with all valid features.
+#[derive(Debug, Clone, Deserialize)]
+struct RawConfig {
+    #[serde(flatten)]
+    raw_experiments: HashMap<String, Value>,
+    #[serde(rename = "$override_groups")]
+    override_groups: Option<OverrideGroupFeature>,
+}
+
+static OVERRIDE_GROUPS: &str = "$override_groups";
+
+impl RawConfig {
+    /// Deserializes the raw config into a list of valid features. Any features that can't be
+    /// successfully deserialized are returned in the `HashMap`.
+    fn features(self) -> (Vec<Feature>, HashMap<String, serde_json::Error>) {
+        let mut ec = HashMap::new();
+        let mut errs = HashMap::new();
+
+        for (name, feature_json) in self.raw_experiments {
+            match serde_json::from_value::<Experiment>(feature_json) {
+                Ok(exp) if name != OVERRIDE_GROUPS => {
+                    ec.insert(name, exp);
+                }
+                Err(err) => {
+                    errs.insert(name, err);
+                }
+                _ => (),
+            }
+        }
+
+        let cfg = ExperimentConfig {
+            experiments: ec,
+            override_groups: self.override_groups.map(|f| f.groups).unwrap_or_default(),
+        };
+
+        (experiment_config_to_features(&cfg), errs)
+    }
+}
 
 #[derive(Deserialize, Debug, Clone)]
 struct Experiment {
     id: u32,
     name: String,
     enabled: bool,
     #[allow(dead_code)] // FIXME: Remove this field?
@@ -1084,135 +1314,176 @@
     value: Option<Value>,
     value_type: Option<ValueType>,
     parent_meg_name: Option<String>,
     parent_hg_name: Option<String>,
     experiment: InnerExperiment,
 }
 
-#[derive(Serialize, Deserialize, Debug, Clone)]
+#[derive(Serialize, Deserialize, Debug, Clone, PartialEq, Eq)]
 #[serde(rename_all = "snake_case")]
 enum ExperimentType {
     DynamicConfig,
     RangeVariant,
-    FeatureRollout, // FIXME: get rid of this after the great RangeVariant takeover.
 }
 
 #[derive(Serialize, Deserialize, Debug, Clone, Copy, PartialEq, Eq)]
-#[serde(rename_all(deserialize = "snake_case"))]
-pub enum BucketVal {
-    #[serde(rename = "user_id")]
-    UserId,
-    #[serde(rename = "device_id")]
-    DeviceId,
-    #[serde(rename = "canonical_url")]
-    CanonicalUrl,
-}
-
-impl fmt::Display for BucketVal {
-    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        match self {
-            BucketVal::UserId => {
-                write!(f, "user_id")
-            }
-            BucketVal::DeviceId => {
-                write!(f, "device_id")
-            }
-            BucketVal::CanonicalUrl => {
-                write!(f, "canonical_url")
-            }
-        }
-    }
-}
-
-impl FromStr for BucketVal {
-    type Err = DeciderError;
-
-    fn from_str(input: &str) -> Result<BucketVal, DeciderError> {
-        match input {
-            "user_id" => Ok(BucketVal::UserId),
-            "device_id" => Ok(BucketVal::DeviceId),
-            "canonical_url" => Ok(BucketVal::CanonicalUrl),
-            _ => Err(DeciderError::IncorrectBucketValString(input.to_string())),
-        }
-    }
-}
-
-#[derive(Serialize, Deserialize, Debug, Clone, PartialEq, Eq)]
 pub enum ValueType {
     Boolean,
     Integer,
     Float,
+    #[serde(alias = "Text")] // FIXME: Remove this once we've moved to `String` in DDG.
     String,
-    Text,
     Map,
+    Null,
+}
+
+impl From<ValueType> for Value {
+    fn from(value_type: ValueType) -> Self {
+        match value_type {
+            ValueType::Boolean => Value::Bool(false),
+            ValueType::Integer => Value::from(0),
+            ValueType::Float => Value::from(0.0),
+            ValueType::String => Value::from(""),
+            ValueType::Map => Value::Object(serde_json::Map::new()),
+            ValueType::Null => Value::Null,
+        }
+    }
 }
 
 impl fmt::Display for ValueType {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
-        match &*self {
+        match self {
             ValueType::Boolean => write!(f, "boolean"),
             ValueType::Integer => write!(f, "integer"),
             ValueType::Float => write!(f, "float"),
             ValueType::String => write!(f, "string"),
-            ValueType::Text => write!(f, "string"),
             ValueType::Map => write!(f, "map"),
+            ValueType::Null => write!(f, "null"),
         }
     }
 }
 
 #[derive(Deserialize, Debug, Clone)]
 struct InnerExperiment {
     experiment_version: u32,
     #[serde(default)]
     variants: Vec<Variant>, // TODO: figure out how to make a variable-length array in a struct, maybe?
     #[serde(default)]
     shuffle_version: u32,
-    bucket_val: Option<BucketVal>,
+    #[serde(rename = "bucket_val")]
+    bucketing_field: Option<ContextField>,
     overrides: Option<Vec<HashMap<String, TargetingTree>>>,
     targeting: Option<TargetingTree>,
 }
 
-fn experiment_to_feature(exp: &Experiment, ec: &ExperimentConfig) -> Feature {
-    let holdout: Option<Box<Feature>> = match &exp.parent_hg_name {
+impl From<&Experiment> for Metadata {
+    fn from(exp: &Experiment) -> Self {
+        Metadata {
+            id: exp.id,
+            name: exp.name.clone(),
+            enabled: exp.enabled,
+            version: exp.experiment.experiment_version,
+            owner: exp.owner.clone(),
+        }
+    }
+}
+
+impl From<&serde_json::Value> for ValueType {
+    fn from(value: &serde_json::Value) -> Self {
+        match value {
+            Value::String(_) => ValueType::String,
+            Value::Object(_) => ValueType::Map,
+            Value::Number(number) => {
+                if number.is_f64() {
+                    ValueType::Float
+                } else {
+                    ValueType::Integer
+                }
+            }
+            Value::Bool(_) => ValueType::Boolean,
+            Value::Null => ValueType::Null,
+            _ => panic!("value {value} are not supported", value = value),
+        }
+    }
+}
+
+fn experiment_to_dynamic_config(exp: &Experiment) -> DynamicConfig {
+    let value = exp
+        .value
+        .clone()
+        .map(Value::from)
+        .unwrap_or_else(|| Value::from(exp.value_type.unwrap_or(ValueType::Null)));
+    let value_type = value.borrow().into();
+
+    DynamicConfig {
+        metadata: exp.into(),
+        value,
+        value_type,
+    }
+}
+
+fn experiment_to_multivariant_choice(exp: &Experiment, ec: &ExperimentConfig) -> RangeVariant {
+    let holdout = match &exp.parent_hg_name {
         None => None,
-        Some(name) => ec.get(name).map(|e| Box::new(experiment_to_feature(e, ec))),
+        Some(name) => ec.experiments.get(name).map(|e| {
+            Box::new(Feature::RangeVariant(experiment_to_multivariant_choice(
+                e, ec,
+            )))
+        }),
     };
 
     let mutex_group = match &exp.parent_meg_name {
         None => None,
-        Some(name) => ec.get(name).map(|e| Box::new(experiment_to_feature(e, ec))),
+        Some(name) => ec.experiments.get(name).map(|e| {
+            Box::new(Feature::RangeVariant(experiment_to_multivariant_choice(
+                e, ec,
+            )))
+        }),
     };
 
-    let variant_set = match exp.experiment_type {
-        ExperimentType::DynamicConfig => None,
-        _ => Some(VariantSet {
-            start_ts: exp.start_ts,
-            stop_ts: exp.stop_ts,
-            shuffle_version: exp.experiment.shuffle_version,
-            variants: exp.experiment.variants.clone(),
-            bucket_val: exp.experiment.bucket_val,
-            holdout,
-            mutex_group,
-        }),
+    let variant_set = VariantSet {
+        start_ts: exp.start_ts,
+        stop_ts: exp.stop_ts,
+        shuffle_version: exp.experiment.shuffle_version,
+        variants: exp.experiment.variants.clone(),
+        bucketing_field: exp
+            .experiment
+            .bucketing_field
+            .clone()
+            .expect("missing bucketing_field for range variant"),
+        holdout,
+        mutex_group,
     };
 
-    Feature {
-        id: exp.id,
-        name: exp.name.clone(),
-        enabled: exp.enabled,
-        feature_type: exp.experiment_type.clone(),
-        version: exp.experiment.experiment_version,
-        owner: exp.owner.clone(),
-        platform_bitmask: 0,
-        value: exp.value.clone(),
-        value_type: exp.value_type.clone(),
+    let overrides = exp.experiment.overrides.as_ref().map(|ov| {
+        ov.iter()
+            .map(|hm| {
+                hm.iter()
+                    .map(|(k, v)| (k.to_string(), v.unroll_groups(&ec.override_groups)))
+                    .collect()
+            })
+            .collect()
+    });
+
+    RangeVariant {
+        metadata: exp.into(),
         emit_event: exp.emit_event,
-        targeting: exp.experiment.targeting.clone(),
-        overrides: exp.experiment.overrides.clone(),
         variant_set,
+        enabled: exp.enabled,
+        targeting: exp.experiment.targeting.clone(),
+        overrides,
+    }
+}
+
+fn experiment_to_feature(exp: &Experiment, ec: &ExperimentConfig) -> Feature {
+    match exp.experiment_type {
+        ExperimentType::DynamicConfig => Feature::DynamicConfig(experiment_to_dynamic_config(exp)),
+        ExperimentType::RangeVariant => {
+            Feature::RangeVariant(experiment_to_multivariant_choice(exp, ec))
+        }
     }
 }
 
 #[cfg(test)]
 mod tests {
     use proptest::prelude::*;
     use serde_json::json;
@@ -1227,40 +1498,39 @@
         String(Option<Value>),
         Map(Option<String>),
     }
 
     fn make_feature() -> Feature {
         let v = Variant {
             name: "enabled".to_string(),
-            lo: 0.0,
-            hi: 0.1,
+            range: 0..100,
         };
-        Feature {
-            id: 1,
-            name: "first_feature".to_string(),
-            enabled: true,
-            feature_type: ExperimentType::RangeVariant,
-            version: 1,
-            owner: "test".to_string(),
-            platform_bitmask: 0,
+
+        Feature::RangeVariant(RangeVariant {
+            metadata: Metadata {
+                id: 1,
+                name: "first_feature".to_string(),
+                enabled: true,
+                version: 1,
+                owner: "test".to_string(),
+            },
             emit_event: true,
-            targeting: None,
-            overrides: None,
-            variant_set: Some(VariantSet {
+            variant_set: VariantSet {
                 start_ts: 0,
                 stop_ts: 2147483648, // 2 ** 31 - far future.
                 shuffle_version: 0,
-                bucket_val: Some(BucketVal::UserId),
+                bucketing_field: ContextField::UserId,
                 variants: vec![v],
                 holdout: None,
                 mutex_group: None,
-            }),
-            value: Some(Value::Null),
-            value_type: None,
-        }
+            },
+            enabled: true,
+            targeting: None,
+            overrides: None,
+        })
     }
 
     fn make_dynamic_config(dc: Dc) -> Feature {
         let name_str: String;
         let value_type: ValueType;
 
         let value: Value = match dc {
@@ -1309,56 +1579,50 @@
                         json!({"v":{"nested_map": {"w":false,"x": 1,"y":"some_string","z":3.0}},"w":false,"x": 1,"y":"some_string","z":3.0})
                     }
                     Some(s) => serde_json::from_str(s).unwrap(),
                 }
             }
         };
 
-        Feature {
-            id: 2,
-            name: name_str + "_dynamic_config",
-            enabled: true,
-            feature_type: ExperimentType::DynamicConfig,
-            version: 1,
-            owner: "test".to_string(),
-            emit_event: true,
-            value: Some(value),
-            value_type: Some(value_type),
-            targeting: None,
-            overrides: None,
-            platform_bitmask: 0,
-            variant_set: None,
-        }
+        Feature::DynamicConfig(DynamicConfig {
+            metadata: Metadata {
+                id: 2,
+                name: name_str + "_dynamic_config",
+                enabled: true,
+                version: 1,
+                owner: "test".to_string(),
+            },
+            value: value,
+            value_type: value_type,
+        })
     }
 
     fn make_experiment(name: String, meg: Option<String>, hg: Option<String>) -> Experiment {
         let c = Variant {
             name: "control".to_string(),
-            hi: 1.0,
-            lo: 0.9,
+            range: 900..1000,
         };
         let t = Variant {
             name: "treatment".to_string(),
-            hi: 0.1,
-            lo: 0.0,
+            range: 0..100,
         };
         Experiment {
             id: 1,
             name,
             experiment_type: ExperimentType::RangeVariant,
             enabled: true,
             owner: "test".to_string(),
             emit_event: true,
             start_ts: 0,
             stop_ts: 2147483648, // 2 ** 31 - far future.
             version: "1".to_string(),
             experiment: InnerExperiment {
                 shuffle_version: 0,
                 variants: vec![t, c],
-                bucket_val: Some(BucketVal::UserId),
+                bucketing_field: Some(ContextField::UserId),
                 experiment_version: 1,
                 targeting: None,
                 overrides: None,
             },
             parent_hg_name: hg,
             parent_meg_name: meg,
             value: None,
@@ -1379,15 +1643,15 @@
     }
 
     fn make_tt(json: String) -> TargetingTree {
         serde_json::from_str(&json).unwrap()
     }
 
     #[test]
-    fn parse_targeting_tree() -> Result<(), String> {
+    fn parse_targeting_tree() {
         let tt1 = make_tt(r#"{"EQ": {"field": "user_id", "values": ["795244"]}}"#.to_string());
         let tt2 = make_tt(r#"{"EQ": {"field": "user_id", "value": "795244"}}"#.to_string());
         let tt3 = make_tt(r#"{"NE": {"field": "user_id", "value": "795244"}}"#.to_string());
         let tt4 = make_tt(r#"{"GT": {"field": "user_id", "value": 7}}"#.to_string());
         let tt5 = make_tt(r#"{"LT": {"field": "user_id", "value": 8}}"#.to_string());
         let tt6 = make_tt(r#"{"GE": {"field": "user_id", "value": 8}}"#.to_string());
         let tt7 = make_tt(r#"{"LE": {"field": "user_id", "value": 8}}"#.to_string());
@@ -1421,54 +1685,53 @@
                    "build_number": 312024,
                    "logged_in": true,
             })
             .to_string(),
         ))
         .unwrap();
 
-        assert!(tt1.eval(&ctx1)?); // ctx1 has user_id 795244, so EQ passes
-        assert!(!tt1.eval(&ctx2)?); // ctx2 has user_id 7, so EQ fails
-        assert!(tt2.eval(&ctx1)?); // tt1 and tt2 are the same, just different representations
-        assert!(!tt2.eval(&ctx2)?); // so should have same results
+        assert!(tt1.eval(&ctx1).unwrap()); // ctx1 has user_id 795244, so EQ passes
+        assert!(!tt1.eval(&ctx2).unwrap()); // ctx2 has user_id 7, so EQ fails
+        assert!(tt2.eval(&ctx1).unwrap()); // tt1 and tt2 are the same, just different representations
+        assert!(!tt2.eval(&ctx2).unwrap()); // so should have same results
 
-        assert!(!tt3.eval(&ctx1)?); // ctx has user_id 795244, so NE against 795244 fails
-        assert!(tt3.eval(&ctx2)?); // ctx2 has user_id 7, so NE against 7 passes
+        assert!(!tt3.eval(&ctx1).unwrap()); // ctx has user_id 795244, so NE against 795244 fails
+        assert!(tt3.eval(&ctx2).unwrap()); // ctx2 has user_id 7, so NE against 7 passes
 
-        assert!(tt4.eval(&ctx1)?); // ctx has user_id 795244, so GT against 7 passes
-        assert!(!tt4.eval(&ctx2)?); // ctx2 has user_id 7, so GT against 7 fails
+        assert!(tt4.eval(&ctx1).unwrap()); // ctx has user_id 795244, so GT against 7 passes
+        assert!(!tt4.eval(&ctx2).unwrap()); // ctx2 has user_id 7, so GT against 7 fails
 
-        assert!(!tt5.eval(&ctx1)?); // ctx has user_id 795244, so LT against 8 passes
-        assert!(tt5.eval(&ctx2)?); // ctx2 has user_id 7, so LT against 8 fails
+        assert!(!tt5.eval(&ctx1).unwrap()); // ctx has user_id 795244, so LT against 8 passes
+        assert!(tt5.eval(&ctx2).unwrap()); // ctx2 has user_id 7, so LT against 8 fails
 
-        assert!(tt6.eval(&ctx1)?); // ctx has user_id 795244, so GE against 8 passes
-        assert!(!tt6.eval(&ctx2)?); // ctx2 has user_id 7, so GE against 8 fails
+        assert!(tt6.eval(&ctx1).unwrap()); // ctx has user_id 795244, so GE against 8 passes
+        assert!(!tt6.eval(&ctx2).unwrap()); // ctx2 has user_id 7, so GE against 8 fails
 
-        assert!(!tt7.eval(&ctx1)?); // ctx has user_id 795244, so LE against 8 fails
-        assert!(tt7.eval(&ctx2)?); // ctx2 has user_id 7, so LE against 8 passes
+        assert!(!tt7.eval(&ctx1).unwrap()); // ctx has user_id 795244, so LE against 8 fails
+        assert!(tt7.eval(&ctx2).unwrap()); // ctx2 has user_id 7, so LE against 8 passes
 
         // test {ALL: [{user_id: "7"} ]}
-        assert!(!tt8.eval(&ctx1)?); // ctx1 has user_id 795244, so EQ fails, so ALL fails
-        assert!(tt8.eval(&ctx2)?); // ctx2 has user_id 7, so EQ passes, so ALL passes
+        assert!(!tt8.eval(&ctx1).unwrap()); // ctx1 has user_id 795244, so EQ fails, so ALL fails
+        assert!(tt8.eval(&ctx2).unwrap()); // ctx2 has user_id 7, so EQ passes, so ALL passes
 
         // same as above, but literal int rather than string
-        assert!(!tt9.eval(&ctx1)?); // ctx1 has user_id 795244, so EQ fails, so ALL fails
-        assert!(tt9.eval(&ctx2)?); // ctx2 has user_id 7, so EQ passes, so ALL passes
+        assert!(!tt9.eval(&ctx1).unwrap()); // ctx1 has user_id 795244, so EQ fails, so ALL fails
+        assert!(tt9.eval(&ctx2).unwrap()); // ctx2 has user_id 7, so EQ passes, so ALL passes
 
         // an impossible targeting tree that asks us to have 2 different user_ids at once.
-        assert!(!imp.eval(&ctx1)?); // ctx1 has user_id 795244, so both EQs fail
-        assert!(!imp.eval(&ctx2)?); // ctx1 has user_id 7, so second EQ fails
-        Ok(())
+        assert!(!imp.eval(&ctx1).unwrap()); // ctx1 has user_id 795244, so both EQs fail
+        assert!(!imp.eval(&ctx2).unwrap()); // ctx1 has user_id 7, so second EQ fails
     }
 
     fn build_decider(
         cfgo: Option<String>,
         fvo: Option<Vec<Feature>>,
         dcvo: Option<Vec<Feature>>,
     ) -> Result<Decider, DeciderInitError> {
-        let fv = match fvo {
+        let mut fv = match fvo {
             None => vec![make_feature()],
             Some(fv) => fv,
         };
         let dcv = match dcvo {
             None => vec![
                 make_dynamic_config(Dc::Bool(None)),
                 make_dynamic_config(Dc::Int(None)),
@@ -1478,15 +1741,24 @@
             ],
             Some(dc) => dc,
         };
         let cfg = match cfgo {
             Some(s) => s,
             None => "darkmode".to_string(), // set a reasonable default here?
         };
-        init(&cfg, [fv, dcv].concat())
+
+        fv.extend(dcv);
+
+        string_to_decisionmakers(&cfg).map(|decisionmakers| Decider {
+            features: fv.into_iter().fold(HashMap::new(), |mut acc, f| {
+                acc.insert(f.metadata().name.to_string(), f);
+                acc
+            }),
+            decisionmakers,
+        })
     }
 
     #[test]
     fn decider_initialization_works() -> Result<(), DeciderInitError> {
         let ctx = make_ctx(None)?;
         let d = build_decider(None, None, None)?;
         assert!(d.choose("first_feature", &ctx, None).is_ok());
@@ -1502,31 +1774,29 @@
             Ok(_) => panic!(),
             Err(e) => println!("got expected error: {:#?}", e),
         }
         Ok(())
     }
 
     #[test]
-    fn test_name_to_decisionmaker() -> Result<(), String> {
-        name_to_decisionmaker("darkmode")?;
-        name_to_decisionmaker("fractional_availability")?;
-        name_to_decisionmaker("locale")?;
-        name_to_decisionmaker("value")?;
-        name_to_decisionmaker("overrides")?;
-        name_to_decisionmaker("targeting")?;
+    fn test_name_to_decisionmaker() {
+        name_to_decisionmaker("darkmode").unwrap();
+        name_to_decisionmaker("fractional_availability").unwrap();
+        name_to_decisionmaker("value").unwrap();
+        name_to_decisionmaker("overrides").unwrap();
+        name_to_decisionmaker("targeting").unwrap();
+
         let res = name_to_decisionmaker("bad-shouldbreak");
-        match res {
-            Ok(_) => Err("obviously bad variant: bad-shouldbreak passed".to_string()),
-            Err(_) => Ok(()),
-        }
+        assert!(res.is_err());
     }
 
     proptest! {
         #[test]
         fn init_decider_doesnt_crash(s in "\\PC*") {
+            #[allow(deprecated)] // testing deprecated function
             let res = init_decider(&s, "../cfgsmall.json");
             match res {
                 Ok(d) => println!("success: {:#?}", d),
                 Err(e) => println!("error: {:#?}", e),
             }
         }
 
@@ -1537,48 +1807,39 @@
             let ctx: Context = make_ctx(Some(v.to_string()))?;
 
             assert!(!imp.eval(&ctx).unwrap());
         }
 
         #[test]
         fn test_meg_hg_invariants(i in 1..1000000000u64) {
-            let d = init_decider(
-                "darkmode overrides targeting holdout mutex_group fractional_availability value",
-                "../test.json").unwrap();
+            let d = Decider::new("../test.json").unwrap();
 
             let ctx: Context = make_ctx(
                 Some(json!({"user_id": i.to_string()}).to_string())
             ).unwrap();
 
             // let's get all 4 test features bucketed, and out of their Results
             let hghalf = d.choose("hghalf", &ctx, None).unwrap();
             let meg2way = d.choose("meg2way", &ctx, None).unwrap();
             let e1 = d.choose("e1", &ctx, None).unwrap();
             let e2 = d.choose("e2", &ctx, None).unwrap();
 
-            match (massage_holdout(hghalf), meg2way) {
+            match (massage_holdout(hghalf), meg2way.variant_name) {
                 // If you're in the holdout, you don't get any experiments
-                ((Some(true), ed), _) => both_no_name(e1, e2, ed),
+                ((Some(true), _), _) => both_no_name(e1, e2),
                 // Regardless of what's going on in the holdout, if the MEG
                 // doesn't give any results, both decisions should have name=None
-                ((_, ed), None) => both_no_name(e1, e2, ed),
-                ((_, ed), Some(mg)) => {
-                    match mg.variant_name {
-                        None => both_no_name(e1, e2, ed), // None == no exps! Shouldn't get here
-                        Some(s) => one_off_one_on(e1, e2, s),
-                    }
-                },
+                (_, None) => both_no_name(e1, e2),
+                (_, Some(mgv)) => one_off_one_on(e1, e2, mgv),
             }
         }
 
         #[test]
         fn test_overrides(i in 6..1000000000u64) {
-            let d = init_decider(
-                "darkmode overrides targeting holdout mutex_group fractional_availability value",
-                "../test.json").unwrap();
+            let d = Decider::new("../test.json").unwrap();
             let ctx1: Context = make_ctx(Some(
                 json!({"user_id": (i * 10).to_string(), "user_is_employee": true}).to_string(),
             )).unwrap();
 
             let ctx2: Context = make_ctx(Some(
                 json!({"user_id": (i * 10 + 1).to_string(),
                        "user_is_employee": false,
@@ -1601,47 +1862,47 @@
                        "build_number": 312024,
                        "logged_in": true,
                 }).to_string(),
             )).unwrap();
 
             println!("test 1");
             // ctx1 is an employee, so it'll get overridden into control in fancy, and never see holdout/meg
-            let control = d.choose("fancy", &ctx1, None).unwrap().unwrap();
-            assert_eq!(control.variant_name, Some("control".to_string()));
+            let control = d.choose("fancy", &ctx1, None).unwrap();
+            assert_eq!(control.variant_name, Some("control_1".to_string()));
             assert_eq!(control.feature_id, 1);
             assert_eq!(control.feature_name, *"fancy");
             assert_eq!(control.feature_version, 4);
-            assert_eq!(control.event_data, vec![format!("1::::1::::fancy::::4::::control::::{}::::user_id::::0::::9668199193::::test", i * 10)]);
+            assert_eq!(control.event_data, vec![format!("1::::1::::fancy::::4::::control_1::::{}::::user_id::::0::::9668199193::::test", i * 10)]);
             assert_eq!(control.events[0].kind, DecisionKind::Override);
             // Json serialization is tested independently. Here we just check that we returned some valid json.
             assert!(serde_json::from_str::<Value>(&control.events[0].json).is_ok());
 
-            let x1 = d.choose("hg", &ctx2, None).unwrap().unwrap();
+            let x1 = d.choose("hg", &ctx2, None).unwrap();
             assert_eq!(x1.variant_name, Some("control_1".to_string()));
             assert_eq!(x1.feature_id, 2);
             assert_eq!(x1.feature_name, *"hg");
             assert_eq!(x1.feature_version, 5);
             assert_eq!(x1.event_data, vec![format!("1::::2::::hg::::5::::control_1::::{}::::user_id::::0::::9668199193::::test", i * 10 + 1)]);
             assert_eq!(x1.events[0].kind, DecisionKind::Override);
             assert!(serde_json::from_str::<Value>(&x1.events[0].json).is_ok());
 
-            let x2 = d.choose("meg", &ctx2, None).unwrap().unwrap();
+            let x2 = d.choose("meg", &ctx2, None).unwrap();
             assert_eq!(x2.variant_name, Some("fancy".to_string()));
             assert_eq!(x2.feature_id, 3);
             assert_eq!(x2.feature_name, *"meg");
             assert_eq!(x2.feature_version, 7);
             // MEGs don't fire exposures since `emit_event` is false in test.json config
             let empty_vec: Vec<String> = vec![];
             assert_eq!(x2.event_data, empty_vec);
             assert!(x2.events.is_empty());
 
             println!("test 2");
             // ctx2 employee=false, so in fancy, "none_hit"s the overrides, passes targeting, goes to holdout-is in control(gets experiments).
             // Passes to the meg, it gets "fancy" treatment, which means it is eligible for this experiment, and gets frac_avail in enabled
-            let exp1 = d.choose("fancy", &ctx2, None).unwrap().unwrap();
+            let exp1 = d.choose("fancy", &ctx2, None).unwrap();
             assert_eq!(exp1.variant_name, Some("exp1".to_string()));
             assert_eq!(exp1.feature_id, 1);
             assert_eq!(exp1.feature_name, *"fancy");
             assert_eq!(exp1.feature_version, 4);
             println!("exp1.event_data={:#?}", exp1.event_data);
             assert_eq!(exp1.event_data, vec![
                 format!("2::::2::::hg::::5::::control_1::::{}::::user_id::::0::::9668199193::::test", i * 10 + 1),
@@ -1652,25 +1913,35 @@
             assert_eq!(exp1.events[1].kind, DecisionKind::FracAvail);
             for event in exp1.events {
                 assert!(serde_json::from_str::<Value>(&event.json).is_ok());
             }
 
 
             println!("test 3");
-            // ctx3 isn't an employee, so misses overrides, and fails targeting, so gets nothing.
-            assert!(d.choose("fancy", &ctx3, None).unwrap().is_none());
+            // ctx3 isn't an employee, so misses overrides, and fails targeting, so gets the default decision.
+            let decision = d.choose("fancy", &ctx3, None).unwrap();
+            assert_eq!(decision, Decision {
+                feature_id: 1,
+                feature_name: "fancy".to_string(),
+                feature_version: 4,
+                variant_name: None,
+                value: Value::Null,
+                value_type: None,
+                event_data: Vec::new(),
+                events: Vec::new(),
+            });
 
             println!("test 4");
             // ctx4 employee=false, so in fancy, "none_hit"s the overrides,
             // passes targeting, goes to holdout-is in control(gets
             // experiments). Passes to the meg, it misses overrides and gets
             // frac_avail'd into the "fancy" treatment, which means it is
             // allowed into the "fancy" experiment, which in turn means it gets
             // bucketed.
-            let fancy = d.choose("fancy", &ctx4, None).unwrap().unwrap();
+            let fancy = d.choose("fancy", &ctx4, None).unwrap();
             println!("fancy={:#?}", fancy);
             assert_eq!(fancy.variant_name, Some("exp1".to_string()));
             assert_eq!(fancy.feature_id, 1);
             assert_eq!(fancy.feature_name, *"fancy");
             assert_eq!(fancy.feature_version, 4);
             assert_eq!(fancy.event_data, vec![
                 format!("2::::2::::hg::::5::::control_1::::{}::::user_id::::0::::9668199193::::test", i * 10 + 3),
@@ -1681,151 +1952,205 @@
             assert_eq!(fancy.events[1].kind, DecisionKind::FracAvail);
             for event in fancy.events {
                 assert!(serde_json::from_str::<Value>(&event.json).is_ok());
             }
         }
 
         fn test_choose_with_optional_identifier_type(i in 0..1000000000u64) {
-            let filepath = "../test.json".to_string();
-            let d = init_decider(
-                "darkmode overrides targeting holdout mutex_group fractional_availability value",
-                &filepath).unwrap();
+            let d = Decider::new("../test.json").unwrap();
 
-            // test bucket_val_string arg
+            // test custom bucketing field arg
             let ctx: Context = make_ctx(Some(
                 json!({"canonical_url": i.to_string()}).to_string(),
             )).unwrap();
 
             println!("test 1");
-            // specify `bucket_val_string` that matches `bucket_val` of experiment's config
-            let c_exp = d.choose("canonical_url_exp", &ctx, Some(BucketVal::CanonicalUrl)).unwrap().unwrap();
+            // specify `bucketing_field_opt` that matches `bucket_val` of experiment's config
+            let c_exp = d.choose("canonical_url_exp", &ctx, Some(ContextField::CanonicalUrl)).unwrap();
             assert_eq!(c_exp.variant_name, Some("enabled".to_string()));
             assert_eq!(c_exp.feature_id, 999);
             assert_eq!(c_exp.feature_name, *"canonical_url_exp");
             assert_eq!(c_exp.feature_version, 8);
             assert_eq!(c_exp.event_data, vec![format!("0::::999::::canonical_url_exp::::8::::enabled::::{}::::canonical_url::::0::::9668199193::::test", i * 10)]);
             assert_eq!(c_exp.events[0].kind, DecisionKind::FracAvail);
             assert!(serde_json::from_str::<Value>(&c_exp.events[0].json).is_ok());
 
             println!("test 2");
-            // specify bucket_val_string that does not match experiment's bucket_val
-            let err = d.choose("canonical_url_exp", &ctx, Some(BucketVal::DeviceId));
-            match err {
-                Ok(_) => panic!(),
-                Err(e) => assert!(matches!(e, DeciderError::IdentifierTypeBucketValMismatch(_,_))),
-            }
+            // specify bucketing_field_opt that does not match experiment's bucket_val
+            let err_res = d.choose("canonical_url_exp", &ctx, Some(ContextField::DeviceId));
+            assert!(matches!(err_res, Err(DeciderError::IdentifierTypeBucketValMismatch(_,_))));
         }
 
         #[test]
         fn test_choose_all(i in 0..1000000000u64) {
-            let filepath = "../test.json".to_string();
-            let d = init_decider(
-                "darkmode overrides targeting holdout mutex_group fractional_availability value",
-                &filepath).unwrap();
+            let filepath = "../test.json";
+            let d = Decider::new(filepath).unwrap();
             let ctx: Context = make_ctx(Some(
                 json!({"user_id": i.to_string(), "canonical_url": i.to_string()}).to_string(),
             )).unwrap();
 
             let file = File::open(filepath)?;
             let reader = BufReader::new(file);
-            let ec: ExperimentConfig = serde_json::from_reader(reader)?;
-            let hm = d.choose_all(&ctx, None).unwrap();
+            let ec = ExperimentConfig {
+                experiments: serde_json::from_reader(reader)?,
+                override_groups: HashMap::new(),
+            };
+            let hm = d.choose_all(&ctx, None);
+            assert_eq!(ec.experiments.len(), hm.len());
             // TODO: come up with something smarter to test here.
             for (k, v) in hm {
                 match v {
                     Err(_) => panic!(), // We shouldn't see any errors
-                    Ok(None) => (), // Normal not to have a decision
-                    Ok(Some(d)) => { // if a decision has a name, must be from the variant names.
+                    Ok(d) => { // if a decision has a name, must be from the variant names.
                         if let Some(name) = d.variant_name { // IFF we got a decision, the names should match.
-                            let exp_conf = ec.get(&k).unwrap();
+                            let exp_conf = ec.experiments.get(&k).unwrap();
                             assert!(exp_conf.experiment.variants.iter().any(|f| f.name == name));
                             assert_eq!(exp_conf.id, d.feature_id);
                             assert_eq!(exp_conf.experiment.experiment_version, d.feature_version);
                             assert_eq!(exp_conf.name, d.feature_name);
 
                         }
                     }
                 }
             }
 
-            // test bucket_val_string arg
+            // test bucketing_field_opt arg
             let ctx1: Context = make_ctx(Some(
                 json!({"canonical_url": i.to_string()}).to_string(),
             )).unwrap();
 
             println!("test 1");
             // retrieve the only `canonical_url` experiment
-            let hm = d.choose_all(&ctx1, Some(BucketVal::CanonicalUrl)).unwrap();
-            let c_exp = &hm["canonical_url_exp"].as_ref().unwrap().as_ref().unwrap();
+            let hm = d.choose_all(&ctx1, Some(ContextField::CanonicalUrl));
+            let c_exp = &hm["canonical_url_exp"].as_ref().unwrap();
             assert_eq!(hm.len(), 1);
             assert_eq!(*(c_exp.variant_name.as_ref().unwrap()),  *"enabled");
             assert_eq!(c_exp.feature_name, *"canonical_url_exp");
             assert_eq!(c_exp.feature_id, 999);
             assert_eq!(c_exp.feature_version, 8);
 
             println!("test 2");
-            // `bucket_val_string`/`bucket_val` does not match any identifier in ctx
+            // `bucketing_field_opt`/`bucket_val` does not match any identifier in ctx
             let ctx2: Context = make_ctx(Some(
                 json!({"device_id": i.to_string()}).to_string(),
             )).unwrap();
 
-            let hm = d.choose_all(&ctx2, Some(BucketVal::CanonicalUrl)).unwrap();
+            let hm = d.choose_all(&ctx2, Some(ContextField::CanonicalUrl));
             assert_eq!(hm.len(), 1);
 
             let err = &hm["canonical_url_exp"];
             match err {
                 Ok(_) => panic!(),
-                Err(e) => assert!(matches!(e, DeciderError::MissingBucketValInContext(_))),
+                Err(e) => assert!(matches!(e, DeciderError::MissingBucketingFieldInContext(_))),
             }
 
             println!("test 4");
             // get empty list since no `device_id` experiments exist in test.json
-            let hm = d.choose_all(&ctx, Some(BucketVal::DeviceId)).unwrap();
+            let hm = d.choose_all(&ctx, Some(ContextField::DeviceId));
             assert!(hm.is_empty());
         }
     }
 
-    fn massage_holdout(hg: Option<Decision>) -> (Option<bool>, Vec<String>) {
-        match hg {
-            None => (None, vec![]),
-            Some(Decision {
-                variant_name: n,
-                event_data: ed,
-                ..
-            }) => (Some(n == Some("holdout".to_string())), ed),
-        }
+    fn massage_holdout(hg: Decision) -> (Option<bool>, Vec<String>) {
+        let Decision {
+            variant_name: n,
+            event_data: ed,
+            ..
+        } = hg;
+        (Some(n == Some("holdout".to_string())), ed)
     }
 
-    fn both_no_name(e1: Option<Decision>, e2: Option<Decision>, _ed: Vec<String>) {
-        assert!(e1.and_then(|d| d.variant_name).is_none());
-        assert!(e2.and_then(|d| d.variant_name).is_none());
+    fn both_no_name(e1: Decision, e2: Decision) {
+        assert!(e1.variant_name.is_none());
+        assert!(e2.variant_name.is_none());
     }
 
-    fn one_off_one_on(e1: Option<Decision>, e2: Option<Decision>, s: String) {
+    fn one_off_one_on(e1: Decision, e2: Decision, expected_variant: String) {
         // This function is highly specific: it depends on being called with
         // e1 == choose("e1") and e2 == choose("e2")
-        match e1.is_none() {
-            true => {
-                assert_eq!(s, "e2".to_string());
-                assert_eq!(e2.unwrap().variant_name, Some("e2treat".to_string()));
-            }
-            false => {
-                assert_eq!(s, "e1".to_string());
-                assert_eq!(e1.unwrap().variant_name, Some("e1treat".to_string()));
+        match e1.variant_name {
+            None => {
+                assert_eq!(expected_variant, "e2".to_string());
+                assert_eq!(e2.variant_name, Some("e2treat".to_string()));
+            }
+            Some(variant_name) => {
+                assert_eq!(expected_variant, "e1".to_string());
+                assert_eq!(variant_name, "e1treat".to_string());
             }
         }
     }
 
     #[test]
-    fn init_decider_works() -> Result<(), DeciderInitError> {
+    fn test_init_decider() {
+        #[allow(deprecated)] // testing deprecated function
         init_decider(
             "darkmode overrides targeting fractional_availability value",
             "../cfg.json",
-        )?;
-        Ok(())
+        )
+        .unwrap();
+    }
+
+    fn check_default_decisionmakers(decider: &Decider) {
+        let decisionmakers: Vec<Decisionmaker> = vec![
+            Decider::darkmode,
+            Decider::overrides,
+            Decider::targeting,
+            Decider::holdout,
+            Decider::mutex_group,
+            Decider::fractional_availability,
+            Decider::value,
+        ];
+
+        check_decisionmakers(decider, decisionmakers);
+    }
+
+    fn check_decisionmakers(decider: &Decider, decisionmakers: Vec<Decisionmaker>) {
+        // decisionmakers are function pointers, so we can compare their addresses.
+        let expected_ptrs: Vec<_> = decisionmakers.iter().map(|dm| *dm as usize).collect();
+        let actual_ptrs: Vec<_> = decider
+            .decisionmakers
+            .iter()
+            .map(|dm| *dm as usize)
+            .collect();
+
+        for (idx, &expected_ptr) in expected_ptrs.iter().enumerate() {
+            assert_eq!(expected_ptr, actual_ptrs[idx]);
+        }
+    }
+
+    #[test]
+    fn test_decider_new() {
+        let decider = Decider::new("../cfg.json").unwrap();
+        check_default_decisionmakers(&decider);
+    }
+
+    #[test]
+    fn test_decider_from_bytes() {
+        let file = File::open("../cfg.json").unwrap();
+        let decider = Decider::from_bytes(file).unwrap();
+        check_default_decisionmakers(&decider);
+    }
+
+    #[test]
+    fn test_with_decisionmakers() {
+        // This should probably be a proptest, but getting proptest to generate function pointers
+        // is really hard.
+        let decisionmakers: Vec<Decisionmaker> = vec![
+            Decider::fractional_availability,
+            Decider::mutex_group,
+            Decider::darkmode,
+        ];
+
+        let file = File::open("../cfg.json").unwrap();
+        let value: Value = serde_json::from_reader(file).unwrap();
+        let decider =
+            Decider::with_decisionmakers(value, "fractional_availability mutex_group darkmode")
+                .unwrap();
+
+        check_decisionmakers(&decider, decisionmakers);
     }
 
     #[test]
     fn holdout_meg_parsing() -> Result<(), DeciderError> {
         let e1 = make_experiment(
             "first".to_string(),
             Some("meg".to_string()),
@@ -1834,55 +2159,144 @@
         let e2 = make_experiment(
             "second".to_string(),
             Some("meg_missing".to_string()),
             Some("hg".to_string()),
         );
         let meg = make_experiment("meg".to_string(), None, None);
         let hg = make_experiment("hg".to_string(), None, None);
-        let ec: ExperimentConfig = HashMap::from([
-            ("first".to_string(), e1),
-            ("second".to_string(), e2),
-            ("meg".to_string(), meg),
-            ("hg".to_string(), hg),
-        ]);
+        let ec: ExperimentConfig = ExperimentConfig {
+            experiments: HashMap::from([
+                ("first".to_string(), e1),
+                ("second".to_string(), e2),
+                ("meg".to_string(), meg),
+                ("hg".to_string(), hg),
+            ]),
+            override_groups: HashMap::new(),
+        };
 
-        let fv: Vec<Feature> = experiment_config_to_features(ec).unwrap();
-        let f1 = fv.iter().find(|&f| f.name == "first").unwrap();
-        let f2 = fv.iter().find(|&f| f.name == "second").unwrap();
-        let fmeg = fv.iter().find(|&f| f.name == "meg").unwrap();
-        let fhg = fv.iter().find(|&f| f.name == "hg").unwrap();
-        assert_eq!(get_fp(f1, FeatureParent::Holdout)?.name, fhg.name);
-        assert_eq!(get_fp(f1, FeatureParent::Meg)?.name, fmeg.name);
+        let fv: Vec<Feature> = experiment_config_to_features(&ec);
+        let f1 = fv.iter().find(|&f| f.metadata().name == "first").unwrap();
+        let f2 = fv.iter().find(|&f| f.metadata().name == "second").unwrap();
+        let fmeg = fv.iter().find(|&f| f.metadata().name == "meg").unwrap();
+        let fhg = fv.iter().find(|&f| f.metadata().name == "hg").unwrap();
+        assert_eq!(
+            get_fp(f1, FeatureParent::Holdout).unwrap().metadata().name,
+            fhg.metadata().name
+        );
+        assert_eq!(
+            get_fp(f1, FeatureParent::Meg).unwrap().metadata().name,
+            fmeg.metadata().name
+        );
         assert!(get_fp(f2, FeatureParent::Meg).is_err());
-        assert_eq!(get_fp(f2, FeatureParent::Holdout)?.name, fhg.name);
+        assert_eq!(
+            get_fp(f2, FeatureParent::Holdout).unwrap().metadata().name,
+            fhg.metadata().name
+        );
         assert!(get_fp(fmeg, FeatureParent::Holdout).is_err());
         assert!(get_fp(fmeg, FeatureParent::Meg).is_err());
         assert!(get_fp(fhg, FeatureParent::Holdout).is_err());
         assert!(get_fp(fhg, FeatureParent::Meg).is_err());
         Ok(())
     }
 
+    #[test]
+    fn test_missing_bool() {
+        let text_dc = json!({
+            "dc_missing_bool": {
+                "id": 1234,
+                "type": "dynamic_config",
+                "version": "1",
+                "enabled": true,
+                "owner": "test",
+                "name": "dc_missing_bool",
+                "experiment": {
+                  "experiment_version": 1
+                },
+                "value": null,
+                "value_type": "Boolean",
+            }
+        });
+
+        let json_str = serde_json::to_string(&text_dc).unwrap();
+        let json_bytes = json_str.as_bytes();
+        let decider = Decider::from_bytes(json_bytes).expect("failed to create decider");
+
+        let values = decider
+            .get_all_values(&Context::default())
+            .expect("no errors");
+        assert_eq!(values["dc_missing_bool"].value, Value::Bool(false));
+    }
+
+    #[test]
+    fn test_bucket_by_arbitrary_field() {
+        let decider = Decider::new("../cfgsmall.json").unwrap();
+
+        let ctx = Context {
+            other_fields: Some(HashMap::from([(
+                "arbitrary_id".to_string(),
+                Value::String("t5_1".to_string()),
+            )])),
+            ..Context::default()
+        };
+
+        let decision = decider.choose("arbitrary_id_exp", &ctx, None).unwrap();
+        assert_eq!("enabled", decision.variant_name.unwrap());
+
+        let ctx = Context {
+            other_fields: Some(HashMap::from([(
+                "arbitrary_id".to_string(),
+                Value::String("t5_10".to_string()),
+            )])),
+            ..Context::default()
+        };
+
+        let decision = decider.choose("arbitrary_id_exp", &ctx, None).unwrap();
+        assert_eq!("control_1", decision.variant_name.unwrap());
+    }
+
+    #[test]
+    fn test_bucket_by_subreddit_id() {
+        let decider = Decider::new("../cfgsmall.json").unwrap();
+
+        let ctx = Context {
+            subreddit_id: Some("t5_1".to_string()),
+            ..Context::default()
+        };
+
+        let decision = decider.choose("subreddit_id_exp", &ctx, None).unwrap();
+        assert_eq!("enabled", decision.variant_name.unwrap());
+
+        let ctx = Context {
+            subreddit_id: Some("t5_5".to_string()),
+            ..Context::default()
+        };
+
+        let decision = decider.choose("subreddit_id_exp", &ctx, None).unwrap();
+        assert_eq!("control_1", decision.variant_name.unwrap());
+    }
+
     enum FeatureParent {
         Meg,
         Holdout,
     }
 
-    fn get_fp(f: &Feature, fp: FeatureParent) -> Result<Feature, DeciderError> {
+    fn get_fp(f: &Feature, fp: FeatureParent) -> Result<Feature, ()> {
         // grab the specified feature_parent(holdout or meg) from a feature, or err trying.
-        if let Some(variant_set) = &f.variant_set {
-            let fpo = match fp {
-                FeatureParent::Meg => variant_set.mutex_group.clone(),
-                FeatureParent::Holdout => variant_set.holdout.clone(),
-            };
-            match fpo {
-                None => Err(DeciderError::FeatureNotFound),
-                Some(feature_parent) => Ok(*feature_parent),
+        match f {
+            Feature::RangeVariant(rv) => {
+                let fpo = match fp {
+                    FeatureParent::Meg => rv.variant_set.mutex_group.clone(),
+                    FeatureParent::Holdout => rv.variant_set.holdout.clone(),
+                };
+                match fpo {
+                    None => Err(()),
+                    Some(feature_parent) => Ok(*feature_parent),
+                }
             }
-        } else {
-            Err(DeciderError::FeatureNotFound)
+            _ => Err(()),
         }
     }
 
     #[test]
     fn get_bool_works() -> Result<(), DeciderInitError> {
         let ctx = make_ctx(None)?;
         let d = build_decider(
@@ -2030,14 +2444,170 @@
             Ok(_) => panic!(),
             Err(e) => println!("got expected error: {:#?}", e),
         }
         Ok(())
     }
 
     #[test]
+    fn no_variant_override() {
+        let cgf = json!({
+            "x0": {
+                "id": 1,
+                "name": "x0",
+                "enabled": true,
+                "owner": "test",
+                "version": "4",
+                "type": "range_variant",
+                "emit_event": true,
+                "experiment": {
+                  "variants": [
+                    {
+                      "name": "enabled",
+                      "size": 1,
+                      "range_end": 1,
+                      "range_start": 0.0
+                    }
+                  ],
+                  "experiment_version": 4,
+                  "shuffle_version": 1,
+                  "bucket_val": "user_id",
+                  "overrides": [
+                    {
+                      "$none": {
+                        "ANY": [
+                          { "EQ": { "field": "user_id", "values": ["t2_1"] } },
+                        ]
+                      }
+                    }
+                  ]
+                },
+                "start_ts": 0,
+                "stop_ts": 2147483647,
+                "value": "range_variant"
+            }
+        });
+
+        let json_str = serde_json::to_string(&cgf).unwrap();
+        let json_bytes = json_str.as_bytes();
+        let decider = Decider::from_bytes(json_bytes).unwrap();
+
+        let ctx = &Context {
+            user_id: Some("t2_1".to_string()),
+            ..Context::default()
+        };
+        let decision = decider.choose("x0", ctx, None).unwrap();
+        assert_eq!(decision.variant_name, None);
+    }
+
+    #[test]
+    fn decider_override_groups() {
+        let cgf = json!({
+            "$override_groups": {
+                "id": 1337,
+                "value": {
+                    "$ads_admins": {
+                        "name": "$ads_admins",
+                        "values": ["t2_ads_id_1", "t2_ads_id_2"],
+                        "field": "user_id"
+                    }
+                },
+                "type": "dynamic_config",
+                "version": "1",
+                "enabled": false,
+                "owner": "test",
+                "name": "$override_group",
+                "value_type": "Map",
+                "experiment": {
+                    "experiment_version": 1
+                }
+            },
+            "x0": {
+                "id": 1,
+                "name": "x0",
+                "enabled": true,
+                "owner": "test",
+                "version": "4",
+                "type": "range_variant",
+                "emit_event": true,
+                "experiment": {
+                  "variants": [
+                    {
+                      "name": "enabled",
+                      "size": 0.5,
+                      "range_end": 0.5,
+                      "range_start": 0.0
+                    },
+                    {
+                      "name": "control_1",
+                      "size": 0.5,
+                      "range_end": 1.0,
+                      "range_start": 0.0
+                    }
+                  ],
+                  "experiment_version": 4,
+                  "shuffle_version": 1,
+                  "bucket_val": "user_id",
+                  "overrides": [
+                    {
+                      "control_1": {
+                        "ANY": [
+                          { "EQ": { "field": "user_id", "values": ["$ads_admins"] } },
+                        ]
+                      }
+                    }
+                  ]
+                },
+                "start_ts": 0,
+                "stop_ts": 2147483647,
+                "value": "range_variant"
+            }
+        });
+
+        let json_str = serde_json::to_string(&cgf).unwrap();
+        let json_bytes = json_str.as_bytes();
+        let decider = Decider::from_bytes(json_bytes).unwrap();
+
+        let ctx = &Context {
+            user_id: Some("t2_ads_id_1".to_string()),
+            ..Context::default()
+        };
+        let decision = decider.choose("x0", ctx, None).unwrap();
+        assert_eq!(&decision.variant_name.unwrap(), "control_1");
+
+        let values = decider.get_all_values(ctx).unwrap();
+        assert_eq!(0, values.len());
+    }
+
+    #[test]
+    fn get_string_with_alias_works() {
+        let text_dc = json!({
+            "text_dc": {
+              "id": 1234,
+              "value": "some_string",
+              "type": "dynamic_config",
+              "version": "1",
+              "enabled": true,
+              "owner": "test",
+              "name": "text_dc",
+              "value_type": "Text", // <--
+              "experiment": {
+                "experiment_version": 1
+              }
+            },
+        });
+
+        let json_str = serde_json::to_string(&text_dc).unwrap();
+        let json_bytes = json_str.as_bytes();
+        let decider = Decider::from_bytes(json_bytes).unwrap();
+
+        let value = decider.get_string("text_dc", &Context::default()).unwrap();
+        assert_eq!("some_string", &value);
+    }
+
+    #[test]
     fn get_map_works() -> Result<(), DeciderInitError> {
         let ctx = make_ctx(None)?;
         let map_dc_str = r#"{"v":{"nested_map": {"w":false,"x": 1,"y":"some_string","z":3.0}},"w":false,"x": 1,"y":"some_string","z":3.0}"#;
         let d = build_decider(
             Some("darkmode fractional_availability value".to_string()),
             None,
             Some(vec![make_dynamic_config(Dc::Map(Some(
@@ -2135,14 +2705,374 @@
         assert!(!value_eq(&v["sn"].clone(), &v["s2"].clone()).unwrap());
         assert!(!value_eq(&v["n"].clone(), &v["s"].clone()).unwrap());
         assert!(!value_eq(&v["bt"].clone(), &v["bf"].clone()).unwrap());
         assert!(!value_eq(&v["n"].clone(), &v["nn"].clone()).unwrap());
         assert!(!value_eq(&v["flt"].clone(), &v["fltn"].clone()).unwrap());
 
         // but here lies madness
-        assert!(value_eq(&v["n"].clone(), &v["tb"].clone()).is_err());
-        assert!(value_eq(&v["n"].clone(), &v["a"].clone()).is_err());
-        assert!(value_eq(&v["a"].clone(), &v["o"].clone()).is_err());
-        assert!(value_eq(&v["a"].clone(), &v["a"].clone()).is_err());
+        assert!(value_eq(&v["n"].clone(), &v["tb"].clone()).is_none());
+        assert!(value_eq(&v["n"].clone(), &v["a"].clone()).is_none());
+        assert!(value_eq(&v["a"].clone(), &v["o"].clone()).is_none());
+        assert!(value_eq(&v["a"].clone(), &v["a"].clone()).is_none());
         Ok(())
     }
+
+    #[test]
+    fn test_get_variants_basic() {
+        let decider = Decider::new("../test.json").unwrap();
+
+        let feature = decider.feature_by_name("canonical_url_exp").unwrap();
+        let expected_variants = vec![
+            Variant {
+                name: "enabled".to_string(),
+                range: 0..1000,
+            },
+            Variant {
+                name: "control_1".to_string(),
+                range: 0..0,
+            },
+        ];
+
+        let actual_variants = match feature {
+            Feature::RangeVariant(rv) => rv.get_variants(),
+            _ => panic!(""),
+        };
+
+        assert_eq!(expected_variants.len(), actual_variants.len());
+        assert!(expected_variants
+            .iter()
+            .all(|item| actual_variants.contains(item)));
+    }
+
+    #[test]
+    fn test_get_variants_group() {
+        let decider = Decider::new("../test.json").unwrap();
+
+        let expected_variants_map = HashMap::from([
+            (
+                "meg2way",
+                vec![
+                    Variant {
+                        name: "e1".to_string(),
+                        range: 0..400,
+                    },
+                    Variant {
+                        name: "e2".to_string(),
+                        range: 600..1000,
+                    },
+                ],
+            ),
+            (
+                "e1",
+                vec![
+                    Variant {
+                        name: "e1treat".to_string(),
+                        range: 0..1000,
+                    },
+                    Variant {
+                        name: "control_1".to_string(),
+                        range: 0..0,
+                    },
+                ],
+            ),
+            (
+                "e2",
+                vec![
+                    Variant {
+                        name: "e2treat".to_string(),
+                        range: 0..1000,
+                    },
+                    Variant {
+                        name: "control_1".to_string(),
+                        range: 0..0,
+                    },
+                ],
+            ),
+        ]);
+
+        let features = vec![
+            decider.feature_by_name("meg2way").unwrap(),
+            decider.feature_by_name("e1").unwrap(),
+            decider.feature_by_name("e2").unwrap(),
+        ];
+
+        features.iter().for_each(|feature| {
+            let expected_variants = expected_variants_map
+                .get(feature.metadata().name.as_str())
+                .unwrap();
+            let actual_variants = match feature {
+                Feature::RangeVariant(rv) => rv.get_variants(),
+                _ => panic!(""),
+            };
+
+            assert_eq!(expected_variants.len(), actual_variants.len());
+            assert!(expected_variants
+                .iter()
+                .all(|item| actual_variants.contains(item)));
+        })
+    }
+
+    #[test]
+    fn test_is_dynamic_config() {
+        let decider = Decider::new("../cfg.json").unwrap();
+        let feature = decider.feature_by_name("dc_int").unwrap();
+
+        assert!(match feature {
+            Feature::DynamicConfig(_) => true,
+            _ => false,
+        });
+    }
+
+    proptest! {
+        #[test]
+        fn test_variant_ser(start in 0..1000u16, end in 0..1000u16) {
+            prop_assume!(start <= end);
+
+            let expected_start = (start as f32) / (TOTAL_BUCKETS as f32);
+            let expected_end = (end as f32) / (TOTAL_BUCKETS as f32);
+
+            let variant = Variant {
+                name: "some variant".to_string(),
+                range: start..end,
+            };
+
+            let jval = serde_json::to_value(variant).unwrap();
+
+            assert_eq!(expected_start, jval["range_start"]);
+            assert_eq!(expected_end, jval["range_end"]);
+        }
+
+        #[test]
+        fn test_variant_des(start in 0.0..1.0f32, end in 0.0..1.0f32) {
+            prop_assume!(start <= end);
+
+            let expected_start = (start * (TOTAL_BUCKETS as f32)) as u16;
+            let expected_end = (end * (TOTAL_BUCKETS as f32)) as u16;
+
+            let jval = json!({
+                "name": "some variant",
+                "range_start": start,
+                "range_end": end,
+            });
+
+            let variant: Variant = serde_json::from_value(jval).unwrap();
+
+            assert_eq!(expected_start, variant.range.start);
+            assert_eq!(expected_end, variant.range.end);
+        }
+    }
+
+    #[test]
+    fn test_partial_load() {
+        let valid_exp = json!({
+            "id": 1,
+            "name": "valid_exp",
+            "enabled": true,
+            "owner": "test",
+            "version": "3",
+            "type": "range_variant",
+            "emit_event": true,
+            "start_ts": 37173982,
+            "stop_ts": 2147483648u32,
+            "experiment": {
+              "variants": [
+                {
+                  "range_start": 0,
+                  "range_end": 1,
+                  "name": "variant_0"
+                }
+              ],
+              "experiment_version": 3,
+              "shuffle_version": 0,
+              "bucket_val": "user_id",
+              "log_bucketing": false
+            },
+        });
+
+        let invalid_exp = json!({
+            "some_key": [1, 2, 3],
+        });
+
+        let config = json!({
+            "valid_exp": valid_exp,
+            "invalid_exp": invalid_exp,
+        });
+
+        let decider_res = Decider::with_decisionmakers(config, Decider::DEFAULT_DECISIONMAKERS);
+        let err = decider_res.expect_err("Constructor should return an error");
+        let (decider, errs) = match err {
+            DeciderInitError::PartialLoad(decider, errs) => (decider, errs),
+            _ => unreachable!("Constructor should return a partial load!"),
+        };
+
+        // Check valid experiment.
+        let ctx = Context {
+            user_id: Some("t2_12345".to_string()),
+            ..Context::default()
+        };
+        let decision = decider.choose("valid_exp", &ctx, None).unwrap();
+        assert_eq!(decision.feature_id, 1);
+        assert_eq!(decision.feature_name, "valid_exp".to_string());
+        assert_eq!(decision.feature_version, 3);
+        assert_eq!(decision.variant_name, Some("variant_0".to_string()));
+
+        // Check errors.
+        assert_eq!(errs.len(), 1);
+        assert!(matches!(
+            errs.get("invalid_exp"),
+            Some(serde_json::Error { .. }),
+        ));
+    }
+
+    mod regression {
+        use crate::{Context, Decider, DecisionKind};
+        use serde_json::json;
+
+        #[test]
+        fn test_holdout_event_regression() {
+            // Holdout groups should emit control events, even when the child feature returns no
+            // variant.
+            let holdout_group = json!({
+                "id": 1,
+                "name": "holdout",
+                "version": "1",
+                "type": "range_variant",
+                "enabled": true,
+                "emit_event": true,
+                "owner": "asdf",
+                "experiment": {
+                    "variants": [{
+                        "name": "holdout",
+                        "range_end": 0.0,
+                        "range_start": 0.0
+                    },{
+                        "name": "control_1",
+                        "range_end": 1.0,
+                        "range_start": 0.0
+                    }],
+                    "experiment_version": 5,
+                    "shuffle_version": 0,
+                    "bucket_val": "user_id",
+                }
+            });
+
+            let child = json!({
+                "id": 2,
+                "name": "child",
+                "version": "1",
+                "type": "range_variant",
+                "enabled": true,
+                "emit_event": true,
+                "owner": "asdf",
+                "parent_hg_name": "holdout",
+                "experiment": {
+                    "variants": [{
+                        "name": "control_1",
+                        "range_end": 0.0,
+                        "range_start": 0.0
+                    }],
+                    "experiment_version": 0,
+                    "shuffle_version": 0,
+                    "bucket_val": "user_id"
+                },
+            });
+
+            let config = json!({
+                "holdout": holdout_group,
+                "child": child,
+            });
+
+            let decider =
+                Decider::from_bytes(serde_json::to_string(&config).unwrap().as_bytes()).unwrap();
+
+            let ctx = Context {
+                user_id: Some("t2_12345".to_string()),
+                ..Context::default()
+            };
+
+            let feature = decider.feature_by_name("child").unwrap();
+            let internal_decision = decider.decide_internal(feature, &ctx).unwrap();
+
+            assert!(internal_decision.variant_name.is_none());
+            assert_eq!("child", internal_decision.feature_name);
+
+            assert_eq!(1, internal_decision.events.len());
+            let event = internal_decision.events.first().unwrap();
+            assert_eq!(DecisionKind::Holdout, event.decision_kind);
+            assert_eq!("holdout", event.feature_name);
+            assert_eq!("control_1", event.variant_name);
+        }
+    }
+}
+
+#[cfg(test)]
+pub(crate) mod generators {
+    use super::*;
+    use proptest::option;
+    use proptest::prelude::*;
+    use uuid::Uuid;
+
+    prop_compose! {
+        pub(crate) fn context_strategy()(
+            user_id in option::of(".*"),
+            locale in option::of(".*"),
+            country_code in option::of(".*"),
+            device_id in option::of(uuid()),
+            canonical_url in option::of(".*"),
+            subreddit_id in option::of(".*"),
+            ad_account_id in option::of(".*"),
+            business_id in option::of(".*"),
+            origin_service in option::of(".*"),
+            user_is_employee in option::of(prop::bool::ANY),
+            logged_in in option::of(prop::bool::ANY),
+            app_name in option::of(".*"),
+            build_number in option::of(prop::num::i32::ANY),
+            oauth_client_id in option::of(".*"),
+            cookie_created_timestamp in option::of(prop::num::i64::ANY),
+            correlation_id in option::of(uuid()),
+            // other_fields omitted for sanity
+        ) -> Context {
+            let device_id = device_id.map(|uuid| uuid.to_string());
+            let correlation_id = correlation_id.map(|uuid| uuid.to_string());
+            Context {
+                user_id,
+                locale,
+                country_code,
+                device_id,
+                canonical_url,
+                subreddit_id,
+                ad_account_id,
+                business_id,
+                origin_service,
+                user_is_employee,
+                logged_in,
+                app_name,
+                build_number,
+                oauth_client_id,
+                cookie_created_timestamp,
+                correlation_id,
+                other_fields: None,
+            }
+        }
+    }
+
+    pub(crate) fn uuid() -> impl Strategy<Value = Uuid> {
+        Just(Uuid::new_v4())
+    }
+
+    pub(crate) fn decision_kind() -> impl Strategy<Value = DecisionKind> {
+        let options: Vec<_> = (0u8..)
+            .map_while(|v| DecisionKind::try_from(v).ok())
+            .collect();
+
+        prop::sample::select(options)
+    }
+
+    // TODO Broaden this strategy (and dependent tests) to include all context fields.
+    pub(crate) fn bucketing_field() -> impl Strategy<Value = ContextField> {
+        prop::sample::select(vec![
+            ContextField::UserId,
+            ContextField::DeviceId,
+            ContextField::CanonicalUrl,
+        ])
+    }
 }
```

### Comparing `reddit_decider-1.2.9/setup.py` & `reddit_decider-1.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="reddit-decider",
     description="Reddit's python experiments framework",
-    long_description="Reddit's Python experiments framework. Bucketing, targeting, overrides, and dynamic config logic is implementated in Rust and wrapped in this Python package.",
+    long_description="""
+    Reddit's Python experiments framework.
+    Bucketing, targeting, overrides, and dynamic config logic is implemented in Rust and wrapped in this Python package.
+    """,
     long_description_content_type="text/markdown",
     url="https://github.snooguts.net/reddit/decider-py",
     project_urls={
         "Documentation": "https://reddit-experiments.readthedocs.io/",
     },
     author="matt knox",
     author_email="matt.knox@reddit.com",
```

### Comparing `reddit_decider-1.2.9/test/integration_test.py` & `reddit_decider-1.3.0/test/integration_test.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.2.9/test/test_rust.py` & `reddit_decider-1.3.0/test/test_rust.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.2.9/test/unit_test.py` & `reddit_decider-1.3.0/test/unit_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         "locale": "us_en",
         "user_is_employee": True,
         "logged_in": None,
         "app_name": "ios",
         "build_number": 1234,
         "country_code": "UA",
         "origin_service": "oss",
-        "auth_client_id": "test",
+        "oauth_client_id": "test",
         "cookie_created_timestamp": 1648859753,
     }
 
     variants = [
         {"range_start": 0.0, "range_end": 0.2, "name": "control_1"},
         {"range_start": 0.2, "range_end": 0.4, "name": "variant_2"},
         {"range_start": 0.4, "range_end": 0.6, "name": "variant_3"},
@@ -180,15 +180,15 @@
                 },
             }
         }
 
         with create_temp_config_file(cfg) as f:
             decider = setup_decider(f.name)
             assert (
-                'Decider initialization failed: Json error: "invalid type: string \\"3248\\"'
+                "Decider initialization failed: Partially loaded Decider: 1 features failed to load: { 'exp_0': invalid type: string \"3248\", expected u32 }."
                 in decider.err()
             )
 
     def test_make_ctx(self):
         ctx = rust_decider.make_ctx(self.valid_ctx_dict)
         self.assertEqual(ctx.err(), None)
 
@@ -196,15 +196,15 @@
         str_fields = [
             "locale",
             "country_code",
             "app_name",
             "device_id",
             "canonical_url",
             "origin_service",
-            "auth_client_id",
+            "oauth_client_id",
         ]
         for str_field in str_fields:
             v_ctx = self.valid_ctx_dict.copy()
             v_ctx[str_field] = 1
             ctx = rust_decider.make_ctx(v_ctx)
             self.assertEqual(f'"{str_field}" type mismatch (string).', ctx.err())
 
@@ -213,15 +213,18 @@
         for bool_field in bool_fields:
             v_ctx = self.valid_ctx_dict.copy()
             v_ctx[bool_field] = "not bool"
             ctx = rust_decider.make_ctx(v_ctx)
             self.assertEqual(f'"{bool_field}" type mismatch (bool).', ctx.err())
 
     def test_make_ctx_int_type_mismatch(self):
-        int_fields = ["build_number", "cookie_created_timestamp"]
+        int_fields = [
+            "build_number",
+            "cookie_created_timestamp",
+        ]
         for int_field in int_fields:
             v_ctx = self.valid_ctx_dict.copy()
             v_ctx[int_field] = "not int"
             ctx = rust_decider.make_ctx(v_ctx)
             self.assertEqual(f'"{int_field}" type mismatch (integer).', ctx.err())
 
     # todo:
@@ -267,15 +270,15 @@
             del ctx["device_id"]
             missing_device_id_ctx = rust_decider.make_ctx(ctx)
 
             choice = decider.choose("genexp_device_id", missing_device_id_ctx)
 
             self.assertEqual(
                 choice.err(),
-                'Missing "device_id" in context for bucket_val = "device_id"',
+                'Missing field "device_id" in context for bucket_val = device_id',
             )
             self.assertEqual(choice.decision(), None)
 
     def test_choose_bucket_val_canonical_url(self):
         with create_temp_config_file(self.canonical_url_exp) as f:
             decider = setup_decider(f.name)
 
@@ -291,15 +294,15 @@
             del ctx["canonical_url"]
             missing_canonical_url_ctx = rust_decider.make_ctx(ctx)
 
             choice = decider.choose("genexp_canonical_url", missing_canonical_url_ctx)
 
             self.assertEqual(
                 choice.err(),
-                'Missing "canonical_url" in context for bucket_val = "canonical_url"',
+                'Missing field "canonical_url" in context for bucket_val = canonical_url',
             )
             self.assertEqual(choice.decision(), None)
 
     def test_choose_bucket_val_canonical_url_with_identifer_type(self):
         with create_temp_config_file(self.canonical_url_exp) as f:
             decider = setup_decider(f.name)
 
@@ -320,30 +323,31 @@
                 feature_name="genexp_canonical_url",
                 ctx=self.ctx,
                 identifier_type="device_id",
             )
 
             self.assertEqual(
                 choice.err(),
-                'Requested identifier_type: "device_id" is incompatible with experiment\'s "bucket_val" = "canonical_url".',
+                'Requested identifier_type "device_id" is incompatible with experiment\'s bucket_val = canonical_url',
             )
             self.assertEqual(choice.decision(), None)
 
     def test_choose_bucket_val_canonical_url_with_incorrect_identifer_type(self):
         with create_temp_config_file(self.canonical_url_exp) as f:
             decider = setup_decider(f.name)
 
             choice = decider.choose(
                 feature_name="genexp_canonical_url",
                 ctx=self.ctx,
                 identifier_type="blah",
             )
 
             self.assertEqual(
-                choice.err(), 'identifier_type: "blah" is not a supported "bucket_val".'
+                choice.err(),
+                'Requested identifier_type "blah" is incompatible with experiment\'s bucket_val = canonical_url',
             )
             self.assertEqual(choice.decision(), None)
 
     def test_choose_with_other_fields_for_targeting(self):
         cfg = self.genexp_0_cfg.copy()
         cfg["genexp_0"]["experiment"].update(
             {"targeting": {"ALL": [{"EQ": {"field": "foo", "values": ["bar"]}}]}}
@@ -381,15 +385,15 @@
             decider = setup_decider(f.name)
             yield decider
 
     def test_choose_feature_not_found(self):
         with self.test_feature_not_found() as d:
             result = d.choose("any", self.ctx)
 
-        self.assertEqual(result.err(), 'Feature "any" not found.')
+        self.assertEqual(result.err(), 'Feature "any" not found')
 
     def test_choose_all(self):
         self.genexp_0_cfg.update(self.additional_2_exp)
 
         with create_temp_config_file(self.genexp_0_cfg) as f:
             decider = setup_decider(f.name)
 
@@ -496,15 +500,15 @@
 
         self.assertEqual(dc.err(), "Decider not found.")
 
     def test_get_bool_feature_not_found(self):
         with self.test_feature_not_found() as d:
             result = d.get_bool("any", self.ctx)
 
-        self.assertEqual(result.err(), 'Feature "any" not found.')
+        self.assertEqual(result.err(), 'Feature "any" not found')
 
     def test_get_int(self):
         int_val = 99
         cfg = {
             "dc_int": {
                 "id": 4393,
                 "value": int_val,
@@ -531,15 +535,15 @@
 
         self.assertEqual(dc.err(), "Decider not found.")
 
     def test_get_int_feature_not_found(self):
         with self.test_feature_not_found() as d:
             result = d.get_int("any", self.ctx)
 
-        self.assertEqual(result.err(), 'Feature "any" not found.')
+        self.assertEqual(result.err(), 'Feature "any" not found')
 
     def test_get_float(self):
         float_val = 3.2
         cfg = {
             "dc_float": {
                 "id": 5393,
                 "value": float_val,
@@ -566,15 +570,15 @@
 
         self.assertEqual(dc.err(), "Decider not found.")
 
     def test_get_float_feature_not_found(self):
         with self.test_feature_not_found() as d:
             result = d.get_float("any", self.ctx)
 
-        self.assertEqual(result.err(), 'Feature "any" not found.')
+        self.assertEqual(result.err(), 'Feature "any" not found')
 
     def test_get_string(self):
         string_val = "some_string"
         cfg = {
             "dc_string": {
                 "id": 6393,
                 "value": string_val,
@@ -601,15 +605,15 @@
 
         self.assertEqual(dc.err(), "Decider not found.")
 
     def test_get_string_feature_not_found(self):
         with self.test_feature_not_found() as d:
             result = d.get_string("any", self.ctx)
 
-        self.assertEqual(result.err(), 'Feature "any" not found.')
+        self.assertEqual(result.err(), 'Feature "any" not found')
 
     def test_get_map(self):
         map_val = {
             "v": {"nested_map": {"w": True, "x": 1, "y": "some_string", "z": 3.0}},
             "w": False,
             "x": 1,
             "y": "some_string",
@@ -642,15 +646,15 @@
 
         self.assertEqual(dc.err(), "Decider not found.")
 
     def test_get_map_feature_not_found(self):
         with self.test_feature_not_found() as d:
             result = d.get_map("any", self.ctx)
 
-        self.assertEqual(result.err(), 'Feature "any" not found.')
+        self.assertEqual(result.err(), 'Feature "any" not found')
 
     def test_get_all_values(self):
         bool_val = True
         cfg_bool = {
             "dc_bool": {
                 "id": 3393,
                 "value": bool_val,
@@ -908,15 +912,15 @@
             )
 
             # set "type" to empty string if "value_type" is missing on cfg
             missing_map_val_res = decisions_dict["dc_missing_value_type"]
             self.assertEqual(missing_map_val_res.err(), None)
             self.assertEqual(
                 missing_map_val_res.value_dict(),
-                {"name": "dc_missing_value_type", "value": False, "type": ""},
+                {"name": "dc_missing_value_type", "value": False, "type": "boolean"},
             )
 
     def test_get_experiment(self):
         with create_temp_config_file(self.genexp_0_cfg) as f:
             decider = setup_decider(f.name)
 
             experiment = decider.get_experiment("genexp_0")
@@ -927,15 +931,14 @@
                 "id": cfg["id"],
                 "name": cfg["name"],
                 "enabled": cfg["enabled"],
                 "type": "range_variant",
                 "owner": cfg["owner"],
                 "emit_event": cfg["emit_event"],
                 "version": cfg["experiment"]["experiment_version"],
-                "platform_bitmask": 0,
                 "value": None,
                 "value_type": None,
                 "targeting": cfg.get("targeting"),
                 "overrides": cfg.get("overrides"),
                 "variant_set": {
                     "start_ts": cfg["start_ts"],
                     "stop_ts": cfg["stop_ts"],
@@ -961,8 +964,8 @@
 
         self.assertEqual(exp.err(), "Decider not found.")
 
     def test_get_experiment_feature_not_found(self):
         with self.test_feature_not_found() as d:
             result = d.get_experiment("any")
 
-        self.assertEqual(result.err(), 'Feature "any" not found.')
+        self.assertEqual(result.err(), 'Feature "any" not found')
```

### Comparing `reddit_decider-1.2.9/test/utils.py` & `reddit_decider-1.3.0/test/utils.py`

 * *Files identical despite different names*

