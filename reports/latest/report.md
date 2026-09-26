# Test report

**OK**

Crucible 1.1.0 by Luciano Federico Pereira

1583 tests · 1581 passed · 2 flagged · 101.023s

Passed 100% · Skipped 0%

## Problems

### Skipped (2)

### `tests/unit/Extension/AssertNoDuplicationTest.php::testTheAbsentToolSaysWhichPackageIsMissing` — skip

```
phpcpd-next is installed, so its absence cannot be observed.
```

### `tests/unit/Extension/DuplicationCheckTest.php::testAskingForTheCheckWithoutTheToolSaysWhichPackageIsMissing` — skip

```
phpcpd-next is installed, so its absence cannot be observed.
```

## Slowest tests

These durations are inflated: xdebug is loaded in coverage mode and hooks every call. Re-run with -d xdebug.mode=off to time the tests instead of the profiler.

1. Both spellings agree on every case · ArchDependency — 9.321s
2. A sibling reference inside the target is not a use · ArchDependency — 3.726s
3. A reference from outside makes a class used · ArchDependency — 3.577s
4. A sibling reference does make a class used · ArchDependency — 3.572s
5. A test slower than its size allows is risky · TestRunner — 3.157s
6. The extension agrees with the incumbents line for line · ExtensionParity — 2.351s
7. An unregistered generator is reported and a registered one is not · ApprovedGeneratorRule — 2.131s
8. Wildcards match within and across segments · ArchRule — 2.079s
9. Every preset produces a context · EnvironmentSimulation — 1.919s
10. Used in nothing is an empty allowlist · ArchRule — 1.793s

## Results

#### tests/unit (2 tests, 96.907s)

##### SkipReasons

| Test | Outcome | Time |
|------|---------|-----:|
| Every skip names a missing capability | ✅ pass | 0.009s |
| No skip hides its reason behind a variable | ✅ pass | 0.003s |

#### Architecture (30 tests, 43.548s)

##### ArchDependency

| Test | Outcome | Time |
|------|---------|-----:|
| A sibling reference inside the target is not a use | ✅ pass | 3.726s |
| A reference out of the target is a use | ✅ pass | 1.415s |
| A sibling reference does make a class used | ✅ pass | 3.572s |
| A reference from outside makes a class used | ✅ pass | 3.577s |
| Both spellings agree on every case | ✅ pass | 9.321s |

##### ArchRule

| Test | Outcome | Time |
|------|---------|-----:|
| A namespace prefix targets everything beneath it | ✅ pass | 0.686s |
| The dependency rule names the offending pair | ✅ pass | 0.706s |
| A real layering rule holds | ✅ pass | 0.712s |
| Ignoring removes classes from the target set | ✅ pass | 0.698s |
| Wildcards match within and across segments | ✅ pass | 2.079s |
| A rule that matches nothing fails | ✅ pass | 0.689s |
| A rule with no expectation fails | ✅ pass | 0.689s |
| The inverse layering rule finds the far side crossing | ✅ pass | 1.791s |
| A violation of the inverse rule is reported | ✅ pass | 1.784s |
| Traits are traits and not classes | ✅ pass | 0.690s |
| A trait namespace is not classes | ✅ pass | 0.687s |
| An enum is an enum | ✅ pass | 0.687s |
| Backing is part of the shape | ✅ pass | 1.373s |
| An int backed enum is not string backed | ✅ pass | 0.686s |
| An unbacked enum is backed by nothing | ✅ pass | 1.372s |
| Extending and implementing nothing | ✅ pass | 1.375s |
| Strict equality is read from the source | ✅ pass | 0.686s |
| Used in nothing is an empty allowlist | ✅ pass | 1.793s |
| Every class is named as its path implies | ✅ pass | 0.684s |
| Methods are checked only where they are declared | ✅ pass | 0.686s |
| An undocumented method is reported | ✅ pass | 0.686s |
| Properties skip promoted ones | ✅ pass | 0.686s |

##### rules.pest

| Test | Outcome | Time |
|------|---------|-----:|
| Event objects are immutable | ✅ pass | 0.005s |
| The impact tier never reaches the browser tier | ✅ pass | 0.004s |
| The retrigger endpoint stays inside the watch tier | ✅ pass | 0.006s |

#### Browser (84 tests, 18.598s)

##### Browsing

| Test | Outcome | Time |
|------|---------|-----:|
| Explicitly disabled means skip | ✅ pass | 0.001s |
| Relative urls are a named refusal | ✅ pass | 0.001s |
| Failure screenshot is null without a visit | ✅ pass | 0.001s |
| Failure screenshot writes the png | ✅ pass | 0.644s |
| A missing screenshot says why and only a dead session is a precondition | ✅ pass | 0.001s |

##### DriverSession

| Test | Outcome | Time |
|------|---------|-----:|
| Drives a real browser end to end | ✅ pass | 0.635s |
| The interaction surface against a real page | ✅ pass | 0.779s |

##### EnvironmentSimulation

| Test | Outcome | Time |
|------|---------|-----:|
| Device city dark mode and overrides | ✅ pass | 0.779s |
| Every preset produces a context | ✅ pass | 1.919s |

##### FrameBuffer

| Test | Outcome | Time |
|------|---------|-----:|
| Frames emerge only when complete | ✅ pass | 0.001s |
| Several frames in one chunk | ✅ pass | 0.001s |
| Garbage payload is a named protocol error | ✅ pass | 0.001s |

##### FrameStream

| Test | Outcome | Time |
|------|---------|-----:|
| Round trips a message | ✅ pass | 0.001s |
| Round trips several frames in sequence | ✅ pass | 0.001s |
| Short length prefix is a named protocol error | ✅ pass | 0.001s |
| Truncated payload is a named protocol error | ✅ pass | 0.001s |
| Non json payload is a named protocol error | ✅ pass | 0.001s |

##### HealthChecks

| Test | Outcome | Time |
|------|---------|-----:|
| Console log semantics | ✅ pass | 0.676s |
| Java script error semantics | ✅ pass | 0.125s |
| Accessibility via axe | ✅ pass | 0.551s |
| Screenshot bytes are png | ✅ pass | 0.129s |

##### InProcessServer

| Test | Outcome | Time |
|------|---------|-----:|
| Served requests share the test process state | ✅ pass | 0.748s |

##### Inertia

| Test | Outcome | Time |
|------|---------|-----:|
| The server rendered page is read from the dom | ✅ pass | 0.578s |
| A client side visit is seen though data page never changes | ✅ pass | 0.450s |
| A non inertia page is named not mistaken for a failed match | ✅ pass | 0.095s |

##### InitScript

| Test | Outcome | Time |
|------|---------|-----:|
| An init script on the context runs before page scripts | ✅ pass | 0.581s |
| An init script applies to every page in the context | ✅ pass | 0.162s |

##### InteractionTail

| Test | Outcome | Time |
|------|---------|-----:|
| Drag attach key down frames and submit | ✅ pass | 0.984s |
| The visit fan out surface | ✅ pass | 0.739s |

##### JsValue

| Test | Outcome | Time |
|------|---------|-----:|
| Scalars | ✅ pass | 0.001s |
| The probe pinned object shape | ✅ pass | 0.001s |
| Unknown envelope is a named error | ✅ pass | 0.001s |

##### Livewire

| Test | Outcome | Time |
|------|---------|-----:|
| A components state is read from its snapshot | ✅ pass | 1.148s |
| A round trip is waited for and changes the state | ✅ pass | 1.311s |
| A component can be addressed by name | ✅ pass | 0.267s |

##### NetworkIdle

| Test | Outcome | Time |
|------|---------|-----:|
| A page that settles returns once it is quiet | ✅ pass | 0.796s |
| A wait outlasts a request that has not started yet | ✅ pass | 0.707s |
| A page that never goes quiet is a named failure | ✅ pass | 1.631s |
| A failed request still ends the wait | ✅ pass | 0.427s |

##### PageAssertionsSurface

| Test | Outcome | Time |
|------|---------|-----:|
| The url decomposes into every component the surface exposes | ✅ pass | 0.004s |
| Every url negation disagrees with its positive | ✅ pass | 0.001s |
| An absent url component reads as empty rather than null | ✅ pass | 0.001s |
| Url is compares the whole url or just the path | ✅ pass | 0.001s |
| Path prefix suffix and fragment prefix read the decomposed part | ✅ pass | 0.001s |
| Query parameters are split and percent decoded | ✅ pass | 0.001s |
| A url with no query has no parameters | ✅ pass | 0.001s |
| Title and text comparisons both directions | ✅ pass | 0.001s |
| Text reads from body for the unscoped form | ✅ pass | 0.001s |
| Attribute comparisons including absence | ✅ pass | 0.001s |
| Form state reads through the field grammar | ✅ pass | 0.001s |
| Select and indeterminate state go through the matched elements | ✅ pass | 0.001s |
| Buttons ask the target grammar rather than the field grammar | ✅ pass | 0.001s |
| Presence and visibility are different questions | ✅ pass | 0.001s |
| Count reads the matched elements and refuses a non integer | ✅ pass | 0.001s |
| Links are matched by visible text with quotes escaped | ✅ pass | 0.001s |
| Source assertions read the raw content | ✅ pass | 0.001s |
| Script compares strictly and defaults to true | ✅ pass | 0.001s |
| Inertia props resolve through dot paths including list indexes | ✅ pass | 0.001s |
| A page that is not inertia says so rather than not matching | ✅ pass | 0.001s |
| Livewire state is read from the snapshot the component carries | ✅ pass | 0.001s |
| A page with no livewire component is null rather than empty | ✅ pass | 0.001s |
| Wire click waits for the cycle it started | ✅ pass | 0.001s |
| Only log type console entries trip the console check | ✅ pass | 0.001s |
| Java script errors and smoke are the same check | ✅ pass | 0.001s |
| Every assertion returns the page so they chain | ✅ pass | 0.001s |

##### PageAssertions

| Test | Outcome | Time |
|------|---------|-----:|
| The assertion surface against a real page | ✅ pass | 0.794s |
| Failures land in the assertion machinery | ✅ pass | 0.132s |

##### RelativeVisit

| Test | Outcome | Time |
|------|---------|-----:|
| Without a handler a relative visit is a named error | ✅ pass | 0.001s |
| A misconfigured handler class is a named error | ✅ pass | 0.001s |
| Relative visits serve through the handler and share the world | ✅ pass | 0.146s |

##### Selector

| Test | Outcome | Time |
|------|---------|-----:|
| Data test shorthand | ✅ pass | 0.001s |
| Css passes through | ✅ pass | 0.001s |
| Bare words mean visible text | ✅ pass | 0.001s |
| Bare html element names stay elements | ✅ pass | 0.001s |
| Fields try name id and data test | ✅ pass | 0.001s |
| Explicit field selectors pass through | ✅ pass | 0.001s |

##### SessionGate

| Test | Outcome | Time |
|------|---------|-----:|
| The tier is off by default | ✅ pass | 0.001s |
| Default state is a named error naming the config line | ✅ pass | 0.001s |
| Explicitly disabled is its own named state | ✅ pass | 0.001s |
| Enabled without playwright names the exact commands | ✅ pass | 0.001s |
| Builder carries the browser block | ✅ pass | 0.001s |
| Engine maps to playwright types | ✅ pass | 0.001s |

##### VisitDialect.pest

| Test | Outcome | Time |
|------|---------|-----:|
| It may visit a page and chain assertions | ✅ pass | 0.611s |
| It refuses relative urls until a server bridge exists | ✅ pass | 0.001s |

#### Server (9 tests, 0.005s)

##### CgiVariables

| Test | Outcome | Time |
|------|---------|-----:|
| The method is uppercased and the uri kept | ✅ pass | 0.001s |
| The host falls back to the loopback when no host header arrives | ✅ pass | 0.001s |
| The host header wins when it arrives | ✅ pass | 0.001s |
| Headers become uppercased underscored http variables | ✅ pass | 0.001s |
| The content type is carried both prefixed and unprefixed | ✅ pass | 0.001s |
| A response header keeps its hyphenated title casing | ✅ pass | 0.001s |
| The headers the renderer owns are dropped | ✅ pass | 0.001s |
| A non iterable or empty named entry is skipped rather than fatal | ✅ pass | 0.001s |
| The last value of a repeated header wins | ✅ pass | 0.001s |

#### PHPStan (17 tests, 14.173s)

##### ApprovedEvalRule

| Test | Outcome | Time |
|------|---------|-----:|
| An unapproved eval is reported and an approved one is not | ✅ pass | 1.646s |

##### ApprovedGeneratorRule

| Test | Outcome | Time |
|------|---------|-----:|
| An unregistered generator is reported and a registered one is not | ✅ pass | 2.131s |

##### DataRowRules

| Test | Outcome | Time |
|------|---------|-----:|
| Every mistake is reported and nothing else | ✅ pass | 1.753s |

##### ExtensionBlackBox

| Test | Outcome | Time |
|------|---------|-----:|
| The fixture analyses to exactly the sentinel | ✅ pass | 1.647s |
| A spread each leaves the value to the items | ✅ pass | 1.540s |
| Scoped uses in resolves through ancestor pest configs | ✅ pass | 1.541s |
| The method level magic and mockery surfaces resolve | ✅ pass | 1.541s |

##### ExtensionParity

| Test | Outcome | Time |
|------|---------|-----:|
| The extension agrees with the incumbents line for line | ✅ pass | 2.351s |

##### UsesResolver

| Test | Outcome | Time |
|------|---------|-----:|
| Resolves imports aliases and both call spellings | ✅ pass | 0.014s |
| Group and comma list imports resolve as php reads them | ✅ pass | 0.001s |
| A scoped registration reads group imports too | ✅ pass | 0.001s |
| Namespace relative and string literal arguments | ✅ pass | 0.001s |
| Foreign uses spellings are ignored | ✅ pass | 0.001s |
| A scoped registration is the whole chain and only a chain with in | ✅ pass | 0.001s |
| Only class references count and each namespace resolves its own | ✅ pass | 0.001s |
| A source cut off mid statement reads what it can and never fails | ✅ pass | 0.002s |
| A file without uses resolves to nothing | ✅ pass | 0.001s |

#### Runner (91 tests, 4.928s)

##### ExpectedOutcome

| Test | Outcome | Time |
|------|---------|-----:|
| An expected skip that skips passes | ✅ pass | 0.006s |
| An expected skip that does not skip fails | ✅ pass | 0.002s |
| The declared reason fragment must appear in the skip reason | ✅ pass | 0.002s |
| A matching reason fragment passes | ✅ pass | 0.002s |
| An expected incomplete that is incomplete passes | ✅ pass | 0.002s |
| An expected incomplete that skips fails naming both outcomes | ✅ pass | 0.002s |
| Only skip and incomplete can be expected | ✅ pass | 0.001s |

##### IssueCollector

| Test | Outcome | Time |
|------|---------|-----:|
| Captures all three kinds without disturbing the test | ✅ pass | 0.005s |
| Silenced errors are not counted | ✅ pass | 0.001s |
| Deprecations triggered in project code are self | ✅ pass | 0.001s |
| Baselined deprecations are suppressed at capture | ✅ pass | 0.001s |
| Drain resets per test but tallies accumulate | ✅ pass | 0.001s |

##### Repetition

| Test | Outcome | Time |
|------|---------|-----:|
| Repetitions are adjacent per test not per group | ✅ pass | 0.003s |
| Anything under two leaves the plan untouched | ✅ pass | 0.001s |
| The group keeps its name and lifecycle hooks | ✅ pass | 0.001s |

##### ResultCache

| Test | Outcome | Time |
|------|---------|-----:|
| Round trip preserves outcome history and duration | ✅ pass | 0.004s |
| Missing file loads as empty cache | ✅ pass | 0.001s |
| Corrupt file loads as empty cache | ✅ pass | 0.001s |
| Incompatible version is discarded not misread | ✅ pass | 0.001s |
| Unknown outcome values are skipped on load | ✅ pass | 0.001s |
| History is bounded most recent first | ✅ pass | 0.001s |

##### RetryAndQuarantine

| Test | Outcome | Time |
|------|---------|-----:|
| A pass on retry is flaky not silently green | ✅ pass | 0.009s |
| Backoff delays shape up | ✅ pass | 0.001s |
| The cli count override keeps the configured shape | ✅ pass | 0.001s |
| The runner actually pauses between attempts | ✅ pass | 0.064s |
| A retry attribute carries its own backoff | ✅ pass | 0.034s |
| The retry budget runs out | ✅ pass | 0.002s |
| A retry attribute overrides the run wide budget | ✅ pass | 0.002s |
| Skips are never retried | ✅ pass | 0.002s |
| The quarantined attribute marks the event | ✅ pass | 0.002s |
| The configuration quarantine list matches by file and name | ✅ pass | 0.002s |
| The flakiness log tallies from the stream | ✅ pass | 0.005s |

##### Scheduler

| Test | Outcome | Time |
|------|---------|-----:|
| Declared order is untouched | ✅ pass | 0.007s |
| Reverse reverses groups and tests within groups | ✅ pass | 0.001s |
| Random order is replayable from its seed | ✅ pass | 0.001s |
| Random order is a permutation of the suite | ✅ pass | 0.001s |
| Defects first weighs recency over severity | ✅ pass | 0.001s |
| Defects first breaks ties toward shorter tests | ✅ pass | 0.001s |
| Duration order runs fastest first | ✅ pass | 0.001s |
| Size order runs small before medium before large before unsized | ✅ pass | 0.001s |
| Reordering never runs a dependent before its dependency | ✅ pass | 0.001s |
| Dataset rows travel as one block through repair | ✅ pass | 0.001s |
| Ignoring dependencies leaves the ordering alone | ✅ pass | 0.001s |

##### Shard

| Test | Outcome | Time |
|------|---------|-----:|
| Shards partition the suite completely and disjointly | ✅ pass | 0.006s |
| Membership is stable when other tests come and go | ✅ pass | 0.002s |
| Malformed shard strings parse to null | ✅ pass | 0.001s |

##### TestDiscoverer

| Test | Outcome | Time |
|------|---------|-----:|
| Routes a plain test php file with only pest calls to the pest dialect | ✅ pass | 0.005s |
| Routes the nested class regression fixture to the pest dialect without crashing | ✅ pass | 0.003s |
| Skips a file with neither a class nor pest calls silently | ✅ pass | 0.001s |
| Routes a file with a top level helper class and top level pest calls to pest dialect | ✅ pass | 0.002s |
| Collects the class when the only pest call declares no test | ✅ pass | 0.010s |

##### TestRunner

| Test | Outcome | Time |
|------|---------|-----:|
| Discovery expands datasets and skips helpers | ✅ pass | 0.022s |
| Outcomes are classified per the spec | ✅ pass | 0.006s |
| Failure carries structured diff on the event | ✅ pass | 0.006s |
| Lifecycle and class hooks | ✅ pass | 0.006s |
| Stream discipline first and last events | ✅ pass | 0.006s |
| Run finish reports complete only for a full finished suite | ✅ pass | 0.004s |
| Stop on halts on the outcome it names | ✅ pass | 0.004s |
| Stop on issue reads what the test emitted not how it ended | ✅ pass | 0.004s |
| Disallowed output is risky and is reported rather than printed | ✅ pass | 0.004s |
| A test slower than its size allows is risky | ✅ pass | 3.157s |

##### TestSelection

| Test | Outcome | Time |
|------|---------|-----:|
| Plain pattern is a case insensitive substring match | ✅ pass | 0.016s |
| Pattern matches class qualified names and wildcards | ✅ pass | 0.001s |
| Pattern reaches dataset spellings | ✅ pass | 0.001s |
| Regular expression patterns pass through verbatim | ✅ pass | 0.001s |
| Group selection includes members and exclusion wins | ✅ pass | 0.001s |
| Emptied groups disappear from the selection | ✅ pass | 0.001s |
| Todo listing selects only marked tests whatever the status | ✅ pass | 0.001s |
| Assignee and issue narrow by the marker fields and imply membership | ✅ pass | 0.001s |
| No wip drops work in progress but keeps todo done and ordinary | ✅ pass | 0.001s |
| Exclude filter is the negated filter | ✅ pass | 0.001s |
| Covers and uses select on declared intent | ✅ pass | 0.002s |
| Requires php extension selects on the declared requirement | ✅ pass | 0.001s |
| Id and file selection tell no filter from a filter that matched nothing | ✅ pass | 0.001s |

##### TimeLimit

| Test | Outcome | Time |
|------|---------|-----:|
| Each declared size carries the specs budget | ✅ pass | 0.002s |
| A declared size wins over the default | ✅ pass | 0.001s |
| Without a size the default decides and nothing is not zero | ✅ pass | 0.001s |

##### TimingOverhead

| Test | Outcome | Time |
|------|---------|-----:|
| Off is the only mode that leaves a duration alone | ✅ pass | 0.002s |
| An empty mode is the clean answer and not a missing one | ✅ pass | 0.001s |
| The notice names the mode and the way out | ✅ pass | 0.001s |
| The mode is read from the ini the extension runs with | ✅ pass | 0.001s |
| The default answer and the asked one agree | ✅ pass | 0.001s |

##### Todo

| Test | Outcome | Time |
|------|---------|-----:|
| A todo never executes and reports incomplete | ✅ pass | 0.004s |
| A wip runs its body like pest | ✅ pass | 0.002s |
| A done todo runs its body normally | ✅ pass | 0.002s |
| The todo marker wins over unmet requirements | ✅ pass | 0.001s |
| The attribute form on a real suite method | ✅ pass | 0.000s |

##### UntestedClassification

| Test | Outcome | Time |
|------|---------|-----:|
| An unmet extension requirement is blocked and reads as missing | ✅ pass | 0.004s |
| An unmet dependency is blocked | ✅ pass | 0.001s |
| A deliberate skip is not blocked | ✅ pass | 0.002s |
| An expected skip reconciling to passed drops the blocked flag | ✅ pass | 0.001s |

#### Process (15 tests, 1.452s)

##### DependencyValues

| Test | Outcome | Time |
|------|---------|-----:|
| Only wanted values are carried | ✅ pass | 0.002s |
| A value round trips into the runner results map | ✅ pass | 0.001s |
| The supervisor can ask after the runner was built | ✅ pass | 0.001s |
| An unserializable value is dropped rather than fatal | ✅ pass | 0.001s |
| Garbage from the artifact is ignored not trusted | ✅ pass | 0.001s |

##### WorkerProtocol

| Test | Outcome | Time |
|------|---------|-----:|
| Test id round trips through its string form | ✅ pass | 0.006s |
| Malformed test id strings parse to null | ✅ pass | 0.001s |
| Manifest round trips through json | ✅ pass | 0.001s |
| Overrides survive the manifest with false distinct from absent | ✅ pass | 0.001s |
| Garbage manifests parse to null | ✅ pass | 0.001s |
| Manifest filter keeps only named tests and their dataset rows | ✅ pass | 0.001s |
| Parser reconstructs a finished test with its failure | ✅ pass | 0.008s |
| Parser round trips the pruning signals | ✅ pass | 0.001s |
| Parser handles start run finish and foreign lines | ✅ pass | 0.001s |

##### WorkerTiming

| Test | Outcome | Time |
|------|---------|-----:|
| A worker does not time its tests through xdebug | ✅ pass | 1.428s |

#### Types (11 tests, 4.684s)

##### TypeExpressionAgreement

| Test | Outcome | Time |
|------|---------|-----:|
| The run time reading agrees with phpstans | ✅ pass | 1.652s |

##### TypeExpression

| Test | Outcome | Time |
|------|---------|-----:|
| A fitting value has no mismatch | ✅ pass | 0.005s |
| Each boundary falls on the side its type says | ✅ pass | 0.002s |
| The first misfit is named by its path | ✅ pass | 0.001s |
| Keys are checked where the type names them | ✅ pass | 0.001s |
| A type that does not read is refused with its position | ✅ pass | 0.001s |
| The refusal points at the token that did not read | ✅ pass | 0.001s |
| Shape keys are read in every quoting and as integers | ✅ pass | 0.001s |
| An unknown generic is refused rather than guessed | ✅ pass | 0.001s |

##### TypeTestRunner

| Test | Outcome | Time |
|------|---------|-----:|
| Every assertion is a test with its own verdict | ✅ pass | 1.517s |
| A name filter keeps only the assertions it names | ✅ pass | 1.503s |

#### Dialect (152 tests, 2.036s)

##### CrucibleDialect.crucible

| Test | Outcome | Time |
|------|---------|-----:|
| \check(fn(): int => 1 + 2)->to be(3); | ✅ pass | 0.083s |
| \check(fn(): ?string => null)->to be null()->group('crucible-dialect'); | ✅ pass | 0.001s |
| \check(fn() => throw new  runtime exception('boom'))->to throw( runtime exception::class, 'boom'); | ✅ pass | 0.002s |
| \check(fn(): array => [1, 2, 3])->to be list()->to have count(3)->to contain(2)->not->to contain(9); | ✅ pass | 0.014s |
| An explicit description wins | ✅ pass | 0.001s |
| A trailing comment is the name | ✅ pass | 0.001s |
| Slashes in strings cannot fool the tokenizer | ✅ pass | 0.002s |
| \check(fn(): bool => true)->to be true(); | ✅ pass | 0.001s |
| \check(fn(): bool => true)->to be true(); #2 | ✅ pass | 0.001s |
| \check(fn(): mixed => $this->from suite config)->to be('loaded'); | ✅ pass | 0.001s |
| Str repeat('ab', 2) = 'abab' | ✅ pass | 0.017s |
| Str repeat('x', 3) = 'xxx' | ✅ pass | 0.001s |
| Strtoupper: uppercases | ✅ pass | 0.001s |
| Strtoupper: leaves digits be | ✅ pass | 0.001s |
| Array sum(an array) = 6 | ✅ pass | 0.001s |
| Array sum(an array) = 0 | ✅ pass | 0.001s |
| Pest-style tests coexist | ✅ pass | 0.004s |
| Described blocks too > it nests as usual | ✅ pass | 0.002s |
| Described blocks too > \check(fn() => $this->dialect)->to be('crucible'); | ✅ pass | 0.001s |

##### DoctestShadow

| Test | Outcome | Time |
|------|---------|-----:|
| Shadows carry namespace expressions and the line map | ✅ pass | 0.008s |
| A one line docblock loses its closer | ✅ pass | 0.001s |
| A global namespace file gets no namespace statement | ✅ pass | 0.001s |
| Crucible mentions outside docblocks are not doctests | ✅ pass | 0.001s |

##### InlineDialect

| Test | Outcome | Time |
|------|---------|-----:|
| One source file yields checks and doctests in declaration order | ✅ pass | 0.027s |
| Only a real doctest makes discovery load a source file | ✅ pass | 0.001s |
| Returns claim compares with equality semantics | ✅ pass | 0.002s |
| Named arguments bind by parameter name | ✅ pass | 0.002s |
| Throws claim accepts the expected exception | ✅ pass | 0.002s |
| Bare check claims the call completes | ✅ pass | 0.002s |
| Instance methods run on a fresh instance | ✅ pass | 0.002s |
| Non public methods are checkable | ✅ pass | 0.003s |
| Free functions are checkable | ✅ pass | 0.002s |
| Doctests run on the expect surface | ✅ pass | 0.005s |
| Group attributes travel into metadata | ✅ pass | 0.002s |
| A wrong returns claim fails the test | ✅ pass | 0.006s |
| An unthrown exception fails the test | ✅ pass | 0.002s |
| An unexpected exception escapes unwrapped | ✅ pass | 0.002s |
| A failing doctest fails the test | ✅ pass | 0.002s |
| Claiming both returns and throws is a load error | ✅ pass | 0.001s |
| A required constructor argument is a load error | ✅ pass | 0.001s |
| A doctest that does not parse is a load error | ✅ pass | 0.001s |
| A doctest that escapes the wrapper is a load error | ✅ pass | 0.001s |
| The wrappers parentheses are neutral over the expression forms | ✅ pass | 0.002s |
| Discovery scans the source includes | ✅ pass | 0.018s |
| Testsuite selection skips inline tests | ✅ pass | 0.001s |
| Source excludes are honored | ✅ pass | 0.001s |

##### PestDialect.pest

| Test | Outcome | Time |
|------|---------|-----:|
| A plain test with bound state | ✅ pass | 0.016s |
| It prefixes descriptions | ✅ pass | 0.001s |
| Chained expectations on one value | ✅ pass | 0.001s |
| Negation applies to exactly one matcher | ✅ pass | 0.001s |
| Common matchers | ✅ pass | 0.003s |
| The argument matchers the parity grid has no axis for | ✅ pass | 0.002s |
| To throw catches and verifies | ✅ pass | 0.001s |
| Datasets spread list rows as arguments with data set "small" | ✅ pass | 0.001s |
| Datasets spread list rows as arguments with data set "zero" | ✅ pass | 0.001s |
| Datasets spread list rows as arguments with data set "negative" | ✅ pass | 0.001s |
| Single-value dataset rows arrive as one argument with data set #0 | ✅ pass | 0.001s |
| Single-value dataset rows arrive as one argument with data set #1 | ✅ pass | 0.001s |
| Inside a describe block > names carry the describe path | ✅ pass | 0.001s |
| Inside a describe block > nested deeper > it still works | ✅ pass | 0.001s |
| A producer | ✅ pass | 0.001s |
| A consumer receives the producer value | ✅ pass | 0.001s |
| A skip is the expected outcome | ✅ pass | 0.000s |
| Expected exceptions via throws | ✅ pass | 0.001s |
| Grouped for selection | ✅ pass | 0.001s |
| The matcher long tail > equality variants | ✅ pass | 0.001s |
| The matcher long tail > comparison and ranges | ✅ pass | 0.001s |
| The matcher long tail > numeric specials and resources | ✅ pass | 0.002s |
| The matcher long tail > string shapes | ✅ pass | 0.002s |
| The matcher long tail > the compact printer declaration registered from  pest.php | ✅ pass | 0.001s |
| The matcher long tail > architecture presets over class strings | ✅ pass | 0.018s |
| The matcher long tail > urls, uuids, json strings | ✅ pass | 0.002s |
| The matcher long tail > identifiers and network formats | ✅ pass | 0.002s |
| The matcher long tail > a hostname is not always a domain | ✅ pass | 0.001s |
| The matcher long tail > sluggable, not already a slug | ✅ pass | 0.001s |
| The matcher long tail > hexadecimal without a prefix | ✅ pass | 0.001s |
| The matcher long tail > class-shape matchers that reflection alone can answer | ✅ pass | 0.036s |
| The matcher long tail > collection membership and shape | ✅ pass | 0.002s |
| The matcher long tail > keys, dot notation, key cases | ✅ pass | 0.002s |
| The matcher long tail > array and object subsets | ✅ pass | 0.002s |
| The wrong-typed-subject refusal > the string matchers refuse a non-string in both forms | ✅ pass | 0.005s |
| The wrong-typed-subject refusal > the key-case matchers refuse a non-iterable in both forms | ✅ pass | 0.003s |
| The wrong-typed-subject refusal > the four calls that reported green where the incumbent reports red | ✅ pass | 0.001s |
| The wrong-typed-subject refusal > each refuses the item rather than the container | ✅ pass | 0.001s |
| The wrong-typed-subject refusal > a key-case matcher answers about any iterable, not only an array | ✅ pass | 0.001s |
| The wrong-typed-subject refusal > the cast family refuses a subject  p h p cannot render as a string | ✅ pass | 0.004s |
| The wrong-typed-subject refusal > a subject  p h p can render is not refused | ✅ pass | 0.001s |
| The wrong-typed-subject refusal > a rendering  p h p endorses is read by default, with no quirk | ✅ pass | 0.001s |
| The wrong-typed-subject refusal > the matchers the incumbent does not guard stay unguarded | ✅ pass | 0.001s |
| Modifiers > each as a property fans matchers over items | ✅ pass | 0.001s |
| Modifiers > each with a callback | ✅ pass | 0.001s |
| Modifiers > sequence pairs expectations with items in order | ✅ pass | 0.001s |
| Modifiers > when and unless gate parts of a chain | ✅ pass | 0.001s |
| Modifiers > json decodes and continues the chain | ✅ pass | 0.001s |
| Higher-order expectations > property access descends into the value | ✅ pass | 0.001s |
| Higher-order expectations > method calls forward to the value | ✅ pass | 0.001s |
| Higher-order expectations > scoped asserts mid-chain | ✅ pass | 0.001s |
| Higher-order expectations > extend registers a custom matcher | ✅ pass | 0.001s |

##### PestDialectConfig.pest

| Test | Outcome | Time |
|------|---------|-----:|
| The scoped extend() provides the binding class | ✅ pass | 0.003s |
| The scoped use() mixes the trait in | ✅ pass | 0.001s |
| Global hooks run before file hooks | ✅ pass | 0.001s |
| A named dataset from  pest.php resolves with data set #0 | ✅ pass | 0.001s |
| A named dataset from  pest.php resolves with data set #1 | ✅ pass | 0.001s |
| A dataset from a  datasets file resolves with its keys with data set "short" | ✅ pass | 0.001s |
| A dataset from a  datasets file resolves with its keys with data set "longer" | ✅ pass | 0.001s |
| A lazy dataset closure materializes at build time with data set #0 | ✅ pass | 0.001s |
| A lazy dataset closure materializes at build time with data set #1 | ✅ pass | 0.001s |
| Bound rows resolve after before each, bound to the instance with data set #0 | ✅ pass | 0.001s |
| Associative rows bind to parameters by name with data set #0 | ✅ pass | 0.001s |
| Named and inline factors multiply with data set "0 / 0" | ✅ pass | 0.001s |
| Named and inline factors multiply with data set "0 / 1" | ✅ pass | 0.001s |
| Named and inline factors multiply with data set "1 / 0" | ✅ pass | 0.001s |
| Named and inline factors multiply with data set "1 / 1" | ✅ pass | 0.001s |
| A dataset composed of multiple yield from sub-generators runs every row with data set #0 | ✅ pass | 0.001s |
| A dataset composed of multiple yield from sub-generators runs every row with data set #1 | ✅ pass | 0.001s |
| A dataset composed of multiple yield from sub-generators runs every row with data set #2 | ✅ pass | 0.001s |
| A dataset composed of multiple yield from sub-generators runs every row with data set #3 | ✅ pass | 0.001s |
| A dataset composed of multiple yield from sub-generators runs every row with data set #4 | ✅ pass | 0.001s |

##### PestDialectLongTail.pest

| Test | Outcome | Time |
|------|---------|-----:|
| A bare description is a todo | ✅ pass | 0.000s |
| It will get a body eventually | ✅ pass | 0.000s |
| Work in progress runs its body like  pest | ✅ pass | 0.005s |
| A body-less wip folds to a todo | ✅ pass | 0.000s |
| A done todo runs its body | ✅ pass | 0.001s |
| It chains methods on the test case | ✅ pass | 0.002s |
| Lazy expectation chains | ✅ pass | 0.001s |
| Higher-order expect receives dataset arguments with data set #0 | ✅ pass | 0.001s |
| Higher-order expect receives dataset arguments with data set #1 | ✅ pass | 0.001s |
| Closure skips are decided after before each | ✅ pass | 0.001s |
| Skip on php with an operator constraint | ✅ pass | 0.001s |
| Skip on windows leaves other platforms running | ✅ pass | 0.001s |
| Fails() inverts the outcome | ✅ pass | 0.001s |
| Throws() accepts a message fragment | ✅ pass | 0.001s |
| Throws unless() with a truthy condition expects nothing | ✅ pass | 0.001s |
| Repeat() runs the body once per repetition with data set "repetition 1 of 3" | ✅ pass | 0.001s |
| Repeat() runs the body once per repetition with data set "repetition 2 of 3" | ✅ pass | 0.001s |
| Repeat() runs the body once per repetition with data set "repetition 3 of 3" | ✅ pass | 0.001s |
| Multiple with() calls form a  cartesian product with data set "0 / 0" | ✅ pass | 0.001s |
| Multiple with() calls form a  cartesian product with data set "0 / 1" | ✅ pass | 0.001s |
| Multiple with() calls form a  cartesian product with data set "1 / 0" | ✅ pass | 0.001s |
| Multiple with() calls form a  cartesian product with data set "1 / 1" | ✅ pass | 0.001s |
| A configured block > inherits the block group and dataset with data set #0 | ✅ pass | 0.001s |
| A configured block > inherits the block group and dataset with data set #1 | ✅ pass | 0.001s |
| A configured block > it applies to every contained test with data set #0 | ✅ pass | 0.001s |
| A configured block > it applies to every contained test with data set #1 | ✅ pass | 0.001s |
| A property chain re-roots to the original subject after each matcher | ✅ pass | 0.001s |
| ->not() works as a method call, not only as a property | ✅ pass | 0.001s |
| A missing property or key is null, not a failure | ✅ pass | 0.001s |
| An uninitialized typed property is null, not a fatal | ✅ pass | 0.001s |
| Not()->to contain() with multiple needles fails only when all are present | ✅ pass | 0.001s |
| Not()->to contain() with multiple needles, all present | ✅ pass | 0.001s |
| Not()->to have keys() fails as soon as any single key is found, even last in the list | ✅ pass | 0.001s |
| Not()->to have properties() fails only when every property is present | ✅ pass | 0.001s |

#### Pest (140 tests, 1.600s)

##### ArchExpectation

| Test | Outcome | Time |
|------|---------|-----:|
| A subject naming nothing passes and says so | ✅ pass | 0.026s |
| The empty case passes under negation as well | ✅ pass | 0.002s |
| A named symbol still answers about itself | ✅ pass | 0.005s |
| A namespace answers for everything beneath it | ✅ pass | 0.003s |
| Both spellings agree | ✅ pass | 0.732s |
| The dependency matchers reach the same source | ✅ pass | 0.012s |
| Documentation and casing answer in the expect spelling too | ✅ pass | 0.005s |
| An enum is not readonly in either spelling | ✅ pass | 0.003s |
| Every plural spelling agrees with its singular | ✅ pass | 0.163s |
| The remaining wrappers answer in the expect spelling | ✅ pass | 0.014s |

##### CurrentTest

| Test | Outcome | Time |
|------|---------|-----:|
| Get throws when no test is running | ✅ pass | 0.003s |
| Get returns whatever was set | ✅ pass | 0.001s |
| Set null clears it | ✅ pass | 0.001s |
| Call reaches a protected method on the running test | ✅ pass | 0.001s |
| Call returning hands back a value of the promised type | ✅ pass | 0.001s |
| Call returning names the method the type and what it got instead | ✅ pass | 0.001s |
| Call returning object accepts any object | ✅ pass | 0.001s |
| Call returning object refuses a non object | ✅ pass | 0.001s |

##### ExpectationFilesystem

| Test | Outcome | Time |
|------|---------|-----:|
| A directory is a directory and not a file | ✅ pass | 0.005s |
| A file is a file and not a directory | ✅ pass | 0.001s |
| A path that does not exist is neither | ✅ pass | 0.001s |
| A readable and writable path answers for its kind only | ✅ pass | 0.001s |
| An unreadable file is not a readable file | ✅ pass | 0.001s |
| An unwritable directory is not a writable directory | ✅ pass | 0.001s |

##### PestBuilderAssertionBridge

| Test | Outcome | Time |
|------|---------|-----:|
| Assertions verified during a test cases tear down bridge into crucibles own counter | ✅ pass | 0.040s |

##### PestBuilderCurrentTestBridge

| Test | Outcome | Time |
|------|---------|-----:|
| Current test is set to the running instance during the test body | ✅ pass | 0.004s |
| Current test is cleared once the test finishes | ✅ pass | 0.002s |

##### PestClassLifecycle

| Test | Outcome | Time |
|------|---------|-----:|
| The class lifecycle wraps the files own hooks | ✅ pass | 0.004s |

##### PestCovers

| Test | Outcome | Time |
|------|---------|-----:|
| Covers names the class under test for every test in the file | ✅ pass | 0.012s |
| The coverage reader actually consumes it | ✅ pass | 0.009s |
| A function target becomes covers function rather than covers class | ✅ pass | 0.002s |
| A target that does not exist is refused rather than covering nothing | ✅ pass | 0.001s |
| Mutates names the source the mutation run narrows to | ✅ pass | 0.002s |
| A mutates target that does not exist is refused | ✅ pass | 0.001s |

##### PestFileSniffer

| Test | Outcome | Time |
|------|---------|-----:|
| Detects a top level it call | ✅ pass | 0.008s |
| Detects a backslash prefixed call | ✅ pass | 0.001s |
| Detects a top level dataset only call | ✅ pass | 0.001s |
| Detects a file whose only test is a top level todo | ✅ pass | 0.001s |
| Detects a file whose only pest spelling is covers | ✅ pass | 0.001s |
| Returns false when there are no entry calls | ✅ pass | 0.001s |
| Ignores a method call of the same name | ✅ pass | 0.001s |
| Ignores a static call of the same name | ✅ pass | 0.001s |
| Ignores a user declared function of the same name | ✅ pass | 0.001s |
| Ignores a call nested inside a closure body | ✅ pass | 0.001s |

##### PestFixture

| Test | Outcome | Time |
|------|---------|-----:|
| Fixture always resolves under the projects tests fixtures | ✅ pass | 0.002s |
| The name is joined to fixtures rather than containing it | ✅ pass | 0.001s |
| A missing fixture is refused and says where it looked | ✅ pass | 0.001s |
| Fixture outside collection says so rather than guessing a directory | ✅ pass | 0.001s |

##### PestRegistry

| Test | Outcome | Time |
|------|---------|-----:|
| Every global refuses outside a file being loaded | ✅ pass | 0.020s |
| Drain folds the files registrations last class winning | ✅ pass | 0.001s |
| Drain closes the bracket so the next call refuses | ✅ pass | 0.001s |
| Begin discards whatever the previous file left | ✅ pass | 0.001s |
| Describe nests the path and pops it even when the body throws | ✅ pass | 0.002s |
| Arch registers an ordinary test and hands back the rule | ✅ pass | 0.001s |
| Check takes its name from a trailing comment when there is one | ✅ pass | 0.001s |
| Check falls back to the source line and then to the line number | ✅ pass | 0.001s |
| A long source line is truncated rather than used whole | ✅ pass | 0.001s |
| Two derived names that agree get an occurrence suffix | ✅ pass | 0.001s |
| A duplicate description is refused the way the incumbent refuses it | ✅ pass | 0.001s |
| Scoping separates names that would otherwise collide | ✅ pass | 0.001s |
| Property refuses every argument shape it cannot run | ✅ pass | 0.001s |
| Property registers one test when the arguments are right | ✅ pass | 0.001s |
| Table names each row from its arguments or its key | ✅ pass | 0.001s |
| Table refuses a row that is not arguments and an expected value | ✅ pass | 0.001s |
| Table names its subject by whatever kind of callable it is | ✅ pass | 0.002s |
| Fixture resolves under the project root and refuses what is not there | ✅ pass | 0.001s |
| Fixture refuses outside a file being collected | ✅ pass | 0.001s |

##### PestScopes

| Test | Outcome | Time |
|------|---------|-----:|
| Keeps every row from multiple composed generators | ✅ pass | 0.010s |
| Preserves string keys from a single generator | ✅ pass | 0.001s |
| Returns a plain array unchanged | ✅ pass | 0.001s |
| Configuration loads outermost first and once per directory | ✅ pass | 0.001s |
| Pest belongs to a configuration file | ✅ pass | 0.001s |
| The nearest declaration of a dataset name wins | ✅ pass | 0.001s |
| An unknown dataset names itself and where to declare it | ✅ pass | 0.001s |
| A closure dataset replays on every use | ✅ pass | 0.001s |
| A closure dataset must return something iterable | ✅ pass | 0.001s |
| A bare registration is selected only when it carries hooks | ✅ pass | 0.001s |
| A glob selects only beneath the declaring directory | ✅ pass | 0.001s |
| The suite declared printer is whatever a configuration chose | ✅ pass | 0.001s |
| Configuring says whether a configuration file is loading | ✅ pass | 0.001s |
| Dataset files beside a pest file are loaded too | ✅ pass | 0.001s |
| Uses is the legacy spelling of the same chain | ✅ pass | 0.008s |
| A dataset needs a file that owns it | ✅ pass | 0.001s |
| A dataset key must be an int or a string | ✅ pass | 0.001s |
| A wildcard glob does not cross a directory separator | ✅ pass | 0.001s |
| A directory outside the root is its own chain | ✅ pass | 0.001s |

##### PestTodoGlobal

| Test | Outcome | Time |
|------|---------|-----:|
| A top level todo carries the same metadata as the chained form | ✅ pass | 0.004s |
| A top level todo carries its assignee issue and note | ✅ pass | 0.002s |

##### RealPhpUnitBootstrap

| Test | Outcome | Time |
|------|---------|-----:|
| The drop in alias is not mistaken for the real package | ✅ pass | 0.002s |
| Bridging leaves the instance alone when the real package is absent | ✅ pass | 0.001s |
| Bridging ignores an instance that cannot count | ✅ pass | 0.001s |
| Configuring looks for php units cli classes and leaves them alone when absent | ✅ pass | 0.001s |
| Configuring is attempted only once | ✅ pass | 0.001s |

##### RealPhpUnitExceptionExpectations

| Test | Outcome | Time |
|------|---------|-----:|
| Was expected returns false when nothing was set | ✅ pass | 0.004s |
| Was expected returns false for an instance without the php unit shape | ✅ pass | 0.001s |
| Was expected returns true when the thrown exception matches the expected class | ✅ pass | 0.001s |
| Was expected fails when the thrown exception is the wrong class | ✅ pass | 0.001s |
| Was expected checks the message contains | ✅ pass | 0.001s |
| Was expected fails when the message does not contain | ✅ pass | 0.001s |
| Was expected checks the message regular expression | ✅ pass | 0.001s |
| Was expected checks the exception code | ✅ pass | 0.001s |
| Was expected fails when the code differs | ✅ pass | 0.001s |
| Verify not unraised is a no op when nothing was expected | ✅ pass | 0.001s |
| Verify not unraised fails when an exception was expected but none was thrown | ✅ pass | 0.001s |
| Was expected finds expectations declared on an ancestor class | ✅ pass | 0.001s |

##### ScopeRegistration

| Test | Outcome | Time |
|------|---------|-----:|
| Extend takes the class and refuses a second one | ✅ pass | 0.004s |
| Use accumulates traits and refuses what is not one | ✅ pass | 0.001s |
| Assign splits names by what they actually are | ✅ pass | 0.001s |
| Assign refuses a name that is neither | ✅ pass | 0.001s |
| In belongs to a configuration file only | ✅ pass | 0.001s |
| In starts null and merges across calls | ✅ pass | 0.001s |
| Groups accumulate in declaration order | ✅ pass | 0.001s |
| Hooks accumulate per kind and answer has hooks | ✅ pass | 0.001s |
| Each hook kind is separate | ✅ pass | 0.001s |
| The printer chain starts | ✅ pass | 0.001s |

##### TestCall

| Test | Outcome | Time |
|------|---------|-----:|
| The declared name carries the it prefix and the describe path | ✅ pass | 0.010s |
| Higher order chaining records methods and property reads | ✅ pass | 0.001s |
| Chaining on a test with a body is a typo rather than a higher order step | ✅ pass | 0.001s |
| Each with call is one cartesian factor and keeps its row keys | ✅ pass | 0.001s |
| With accepts any iterable and materialises it | ✅ pass | 0.001s |
| Skip distinguishes all four of its argument shapes | ✅ pass | 0.001s |
| A closure skip is kept unevaluated with its reason beside | ✅ pass | 0.001s |
| The platform skips agree with this machine | ✅ pass | 0.001s |
| Ci skips read the environment and treat falsey values as not ci | ✅ pass | 0.001s |
| Skip on php understands every operator the spec writes | ✅ pass | 0.001s |
| A constraint naming no version is refused | ✅ pass | 0.001s |
| Todo wip and done carry their status and metadata | ✅ pass | 0.001s |
| Fails records the expectation and its optional fragment | ✅ pass | 0.001s |
| Expects skip and expects incomplete record the outcome they demand | ✅ pass | 0.001s |
| Throws records a class or a fragment and an optional message | ✅ pass | 0.001s |
| Throws if and throws unless are opposites over both condition forms | ✅ pass | 0.001s |
| Repeat takes a positive count and refuses anything else | ✅ pass | 0.001s |
| Groups and dependencies accumulate across calls | ✅ pass | 0.001s |

##### TraitComposer

| Test | Outcome | Time |
|------|---------|-----:|
| No shape ends the process | ✅ pass | 0.396s |
| A collision names both traits and the method | ✅ pass | 0.001s |
| An abstract base names what nobody implements | ✅ pass | 0.001s |
| The composed class carries every trait and the base | ✅ pass | 0.001s |
| The same combination is composed once whatever the order | ✅ pass | 0.001s |
| No traits means no generated class at all | ✅ pass | 0.001s |
| A final base is refused with its name | ✅ pass | 0.001s |

#### PhpUnit (6 tests, 0.007s)

##### ClassLocator

| Test | Outcome | Time |
|------|---------|-----:|
| Excludes the nested class in the real spatie regression fixture | ✅ pass | 0.003s |
| Excludes a class nested inside a closure body | ✅ pass | 0.001s |
| Excludes a class nested inside a function body | ✅ pass | 0.001s |
| Still finds a true top level class | ✅ pass | 0.001s |
| Still excludes an anonymous class | ✅ pass | 0.001s |
| Finds a top level class declared after a nested one | ✅ pass | 0.001s |

#### Property (47 tests, 1.668s)

##### GenOf

| Test | Outcome | Time |
|------|---------|-----:|
| Every drawn value fits its type with data set "a DTO shape" | ✅ pass | 0.150s |
| Every drawn value fits its type with data set "a range" | ✅ pass | 0.005s |
| Every drawn value fits its type with data set "nullable" | ✅ pass | 0.011s |
| Every drawn value fits its type with data set "string keys" | ✅ pass | 0.136s |
| Every drawn value fits its type with data set "a non-empty list of literals" | ✅ pass | 0.037s |
| Every drawn value fits its type with data set "nested" | ✅ pass | 0.048s |
| Every drawn value fits its type with data set "numeric strings" | ✅ pass | 0.036s |
| Every drawn value fits its type with data set "a range open below" | ✅ pass | 0.005s |
| Every drawn value fits its type with data set "a range open above" | ✅ pass | 0.005s |
| Every drawn value fits its type with data set "int keys" | ✅ pass | 0.125s |
| Every drawn value fits its type with data set "any keys" | ✅ pass | 0.096s |
| Every drawn value fits its type with data set "non-empty with keys" | ✅ pass | 0.151s |
| A type with no sound way to draw is refused | ✅ pass | 0.001s |
| A non empty type whose every key php rewrites is refused | ✅ pass | 0.016s |
| A failing property shrinks to the smallest shape | ✅ pass | 0.018s |

##### PropertyDatabase

| Test | Outcome | Time |
|------|---------|-----:|
| A stored sequence replays before any random case | ✅ pass | 0.011s |
| Each check in a test claims its own key | ✅ pass | 0.001s |
| Without a context there is no key and no database | ✅ pass | 0.001s |
| The runner puts the replay data on the event | ✅ pass | 0.002s |
| A clean replay rides the passing finish event | ✅ pass | 0.002s |
| An inert stored sequence is not reported clean | ✅ pass | 0.002s |
| A failing test reports no clean keys | ✅ pass | 0.003s |
| The writer prunes clean and orphaned keys on a complete run | ✅ pass | 0.005s |
| An incomplete run prunes clean keys but never orphans | ✅ pass | 0.001s |
| The database round trips merges and bounds | ✅ pass | 0.001s |

##### PropertyDialect.crucible

| Test | Outcome | Time |
|------|---------|-----:|
| String concatenation is associative | ✅ pass | 0.016s |
| Sorting is idempotent | ✅ pass | 0.013s |
| Json round-trips lists of ints | ✅ pass | 0.014s |

##### Property

| Test | Outcome | Time |
|------|---------|-----:|
| A true property holds | ✅ pass | 0.012s |
| List reversal round trips | ✅ pass | 0.013s |
| A false property is falsified and shrunk to the boundary | ✅ pass | 0.004s |
| Shrinking finds the minimal list | ✅ pass | 0.005s |
| Shrinking survives map | ✅ pass | 0.002s |
| Returning false falsifies | ✅ pass | 0.001s |
| The same seed reproduces the same counterexample | ✅ pass | 0.034s |
| Such that filters and stays shrinkable | ✅ pass | 0.003s |
| An impossible filter is a configuration problem | ✅ pass | 0.614s |
| Generators produce their declared shapes | ✅ pass | 0.009s |
| Integers shrink toward zero not the lower bound | ✅ pass | 0.002s |
| Choice source replays and clamps scripts | ✅ pass | 0.001s |
| Floats stay in range and shape up | ✅ pass | 0.010s |
| Floats shrink to the simplest special value | ✅ pass | 0.002s |
| Narrow float ranges resolve | ✅ pass | 0.026s |
| Narrow float falsifies inside the range and shrinks to its edge | ✅ pass | 0.017s |
| Float rejects a non finite or inverted range | ✅ pass | 0.001s |
| For all needs a generator | ✅ pass | 0.000s |
| Int rejects an inverted range | ✅ pass | 0.000s |

#### Reporting (44 tests, 1.651s)

##### MapView

| Test | Outcome | Time |
|------|---------|-----:|
| The first frame reserves a cell for every test | ✅ pass | 0.102s |
| An unknown total draws nothing | ✅ pass | 0.001s |
| A non animated terminal gets the report and no frame | ✅ pass | 0.011s |
| The report follows the frame | ✅ pass | 0.077s |
| Every outcome gets its own glyph | ✅ pass | 0.058s |
| The frame never changes height | ✅ pass | 0.109s |
| A population larger than the window is paged | ✅ pass | 0.120s |
| A page turn is not throttled | ✅ pass | 0.120s |
| The running test is named on one line | ✅ pass | 0.041s |
| A small suite gets a short frame | ✅ pass | 0.020s |
| The readouts are always present | ✅ pass | 0.021s |
| A terminal too narrow for the frame draws nothing | ✅ pass | 0.002s |
| The frame carries a wall clock | ✅ pass | 0.020s |
| The clock separators pulse with the second | ✅ pass | 0.001s |
| The configuration is named on the frame | ✅ pass | 0.020s |
| The mark cycles through its phases | ✅ pass | 0.001s |
| The frame opens before the run with a note | ✅ pass | 0.068s |
| An opening frame is closed when no run follows | ✅ pass | 0.035s |
| The cursor is never shown while the frame is up | ✅ pass | 0.130s |
| The alternate screen is restored | ✅ pass | 0.058s |

##### Reporters

| Test | Outcome | Time |
|------|---------|-----:|
| Console lifts blocked skips into a quiet untested section | ✅ pass | 0.026s |
| Console colors output only when enabled | ✅ pass | 0.003s |
| Markdown splits untested from skipped and problems | ✅ pass | 0.011s |
| Test dox marks untested distinctly and splits the tally | ✅ pass | 0.004s |
| Test dox renders prettified sections and marks | ✅ pass | 0.002s |
| Team city escapes the service message characters | ✅ pass | 0.007s |
| J unit report is well formed with spec granularity | ✅ pass | 0.010s |
| J unit carries surefire flaky and rerun markup | ✅ pass | 0.001s |
| Markdown report carries summary table problems and escaped cells | ✅ pass | 0.002s |
| The slowest section states when the profiler is what it ranked | ✅ pass | 0.002s |
| Pdf report is well formed and carries the run content | ✅ pass | 0.023s |
| Pdf report title is configurable | ✅ pass | 0.013s |
| Pdf verdict is flaky only on pass after retry | ✅ pass | 0.010s |
| Pdf groups directories once and elides flag only files | ✅ pass | 0.014s |
| The profile lists the slowest tests first | ✅ pass | 0.004s |
| The profile shows each tests share of the run | ✅ pass | 0.001s |
| The profile honours its limit | ✅ pass | 0.001s |
| A profile of nothing prints nothing | ✅ pass | 0.001s |

##### RunModel

| Test | Outcome | Time |
|------|---------|-----:|
| Groups finished tests by file in first seen order | ✅ pass | 0.004s |
| Passed tests are neither problems nor untested | ✅ pass | 0.001s |
| Non passed unblocked tests are problems | ✅ pass | 0.001s |
| Blocked tests are untested not problems regardless of outcome | ✅ pass | 0.001s |
| Untested groups by reason in first seen order | ✅ pass | 0.001s |
| Untested with no reason falls back to a could not run label | ✅ pass | 0.001s |

#### Document (21 tests, 0.423s)

##### PdfPrimitives

| Test | Outcome | Time |
|------|---------|-----:|
| The cursor starts one margin below the page top | ✅ pass | 0.007s |
| A heading places its baseline rule and advance exactly | ✅ pass | 0.021s |
| A line advances by its leading | ✅ pass | 0.001s |
| An indent moves the line right without changing the advance | ✅ pass | 0.001s |
| Ensure breaks exactly at the footer reserve | ✅ pass | 0.001s |
| Measure sums the afm widths and scales by size | ✅ pass | 0.001s |
| Bold uses its own width table | ✅ pass | 0.001s |
| A leader fills the gap with measured dots | ✅ pass | 0.001s |
| A narrow gap gets no leader at all | ✅ pass | 0.001s |
| A disc places every arc control point | ✅ pass | 0.001s |
| A box is a filled rectangle in its own colour | ✅ pass | 0.001s |
| Numbers are two decimal places | ✅ pass | 0.001s |
| Escape protects the string delimiters | ✅ pass | 0.001s |
| Wrap chunks at the fixed pitch column budget | ✅ pass | 0.001s |
| Wrap keeps newlines as rows and normalises crlf | ✅ pass | 0.001s |
| Wrap never drops to zero columns | ✅ pass | 0.001s |
| Bookmarks carry their level title and page | ✅ pass | 0.001s |

##### SampleDocument

| Test | Outcome | Time |
|------|---------|-----:|
| Build includes every known block type exactly once | ✅ pass | 0.008s |
| Toc is the first block | ✅ pass | 0.001s |
| Renders through pdf without throwing | ✅ pass | 0.009s |
| Renders through markdown without throwing | ✅ pass | 0.009s |

#### Renderers (23 tests, 0.263s)

##### JsonRenderer

| Test | Outcome | Time |
|------|---------|-----:|
| Summary counts and problems match the run | ✅ pass | 0.007s |
| All passing run has an empty problems list | ✅ pass | 0.001s |

##### PdfRenderer

| Test | Outcome | Time |
|------|---------|-----:|
| Embeds the jpeg as an x object with dct decode and the jpegs own dimensions | ✅ pass | 0.029s |
| The page that draws the image lists it in its resources and paints it | ✅ pass | 0.001s |
| The same bytes drawn twice embed only once | ✅ pass | 0.001s |
| Non jpeg bytes are rejected | ✅ pass | 0.001s |
| Page break starts a fresh page | ✅ pass | 0.002s |
| Headings produce outline bookmarks | ✅ pass | 0.002s |
| No headings produces no outlines | ✅ pass | 0.001s |
| Toc block renders a table of contents page with shifted page numbers | ✅ pass | 0.003s |
| Toc is ignored unless it is the first block | ✅ pass | 0.001s |
| Svg draws shapes fit to width preserving aspect ratio | ✅ pass | 0.022s |
| Malformed svg markup is rejected | ✅ pass | 0.001s |
| Svg with an unsupported feature is rejected | ✅ pass | 0.001s |
| The tile grid places every column label and stat | ✅ pass | 0.005s |
| A tiles rank decides its dot and colour | ✅ pass | 0.002s |
| The table of contents indents and sizes by level | ✅ pass | 0.002s |
| Toc page numbers are right aligned in the column | ✅ pass | 0.002s |

##### SarifRenderer

| Test | Outcome | Time |
|------|---------|-----:|
| Failed test becomes an error level result at the real call site | ✅ pass | 0.008s |
| Skipped test omits a region when there is no trace frame | ✅ pass | 0.001s |
| Declares both rules up front regardless of what fired | ✅ pass | 0.001s |
| Invocation carries the runs real start and end time | ✅ pass | 0.001s |

##### SarifSchema

| Test | Outcome | Time |
|------|---------|-----:|
| A mixed run validates against the sarif schema | ✅ pass | 0.165s |

#### Support (3 tests, 0.004s)

##### FailureLocation

| Test | Outcome | Time |
|------|---------|-----:|
| Picks the frame matching the tests own declaring file | ✅ pass | 0.003s |
| Falls back to the innermost frame when none matches the test file | ✅ pass | 0.001s |
| Returns null when there is no failure at all | ✅ pass | 0.001s |

#### Svg (50 tests, 0.069s)

##### SvgDocument

| Test | Outcome | Time |
|------|---------|-----:|
| View box is read from the view box attribute | ✅ pass | 0.008s |
| View box falls back to width and height attributes | ✅ pass | 0.001s |
| No view box or dimensions throws | ✅ pass | 0.001s |
| A rect emits the re operator and a fill color | ✅ pass | 0.001s |
| A rounded rect emits every bezier corner coordinate | ✅ pass | 0.001s |
| A single radius rounds both axes | ✅ pass | 0.001s |
| A circle emits every bezier arc coordinate | ✅ pass | 0.001s |
| An ellipse uses each radius on its own axis | ✅ pass | 0.001s |
| A non positive radius falls back to the re operator | ✅ pass | 0.001s |
| A polygon closes its path | ✅ pass | 0.001s |
| A polyline does not close | ✅ pass | 0.001s |
| A line draws as a stroke by default since lines have no fill area | ✅ pass | 0.001s |
| A path with an arc renders curve operators | ✅ pass | 0.016s |
| Fill and stroke both present use the b operator | ✅ pass | 0.001s |
| Fill none with stroke uses the s operator | ✅ pass | 0.001s |
| Fill rule evenodd uses the star operator | ✅ pass | 0.001s |
| Stroke width emits the w operator | ✅ pass | 0.001s |
| Rgb function color syntax | ✅ pass | 0.001s |
| Short hex color syntax | ✅ pass | 0.001s |
| Inline style attribute is honored for presentation properties | ✅ pass | 0.001s |
| A translate transform nests a q cm block | ✅ pass | 0.001s |
| A scale transform | ✅ pass | 0.001s |
| Fill is inherited from an ancestor group | ✅ pass | 0.001s |
| A child overrides the inherited fill | ✅ pass | 0.001s |
| An unused defs block renders nothing | ✅ pass | 0.001s |
| Default fill is black when unspecified | ✅ pass | 0.001s |
| Gradient fill throws | ✅ pass | 0.001s |
| Filter attribute throws | ✅ pass | 0.001s |
| Clip path attribute throws | ✅ pass | 0.001s |
| Mask attribute throws | ✅ pass | 0.001s |
| Text element throws | ✅ pass | 0.001s |
| Embedded image element throws | ✅ pass | 0.001s |
| Style element throws | ✅ pass | 0.001s |
| Non one opacity throws | ✅ pass | 0.001s |
| Full opacity does not throw | ✅ pass | 0.001s |

##### SvgPathData

| Test | Outcome | Time |
|------|---------|-----:|
| Absolute move and line commands with close | ✅ pass | 0.006s |
| Relative move and line commands produce the same shape as absolute | ✅ pass | 0.001s |
| Implicit linetos following a moveto | ✅ pass | 0.001s |
| Horizontal and vertical line commands | ✅ pass | 0.001s |
| Cubic bezier command | ✅ pass | 0.001s |
| Smooth cubic reflects the previous control point | ✅ pass | 0.001s |
| Smooth cubic with no preceding cubic uses the current point as the reflection | ✅ pass | 0.001s |
| Quadratic bezier is upgraded to cubic | ✅ pass | 0.001s |
| Multiple subpaths from separate move commands | ✅ pass | 0.001s |
| A zero radius arc degenerates to a straight line | ✅ pass | 0.001s |
| Malformed path data throws | ✅ pass | 0.001s |
| Arc to beziers matches the known quarter circle kappa constant | ✅ pass | 0.001s |
| A half circle arc splits into two segments | ✅ pass | 0.001s |
| Large arc flag changes arc extent | ✅ pass | 0.001s |
| Degenerate same start and end arc in path data | ✅ pass | 0.001s |

#### Blocks (17 tests, 0.026s)

##### Badge

| Test | Outcome | Time |
|------|---------|-----:|
| Ok when nothing failed and nothing was flaky | ✅ pass | 0.003s |
| Flaky when a passed only on retry and nothing failed | ✅ pass | 0.001s |
| Failed wins over flaky when both apply | ✅ pass | 0.001s |
| Errored alone is also failed | ✅ pass | 0.001s |
| Skips and incompletes never change the verdict | ✅ pass | 0.001s |
| Sample returns a valid instance | ✅ pass | 0.001s |

##### FoldingTree

| Test | Outcome | Time |
|------|---------|-----:|
| Single child chains collapse into one label | ✅ pass | 0.011s |
| Absolute paths fold instead of recursing forever | ✅ pass | 0.001s |
| Absolute siblings still split at their common root | ✅ pass | 0.001s |
| Siblings order by descending subtree time | ✅ pass | 0.001s |
| Sub threshold tail folds | ✅ pass | 0.001s |
| A fold of exactly one stays visible | ✅ pass | 0.001s |
| A directory holding a flagged file never folds | ✅ pass | 0.001s |
| Sample returns a valid instance | ✅ pass | 0.001s |

##### Image

| Test | Outcome | Time |
|------|---------|-----:|
| Carries the jpeg bytes and no explicit width by default | ✅ pass | 0.002s |
| Width can narrow the default fit to content width | ✅ pass | 0.001s |
| Sample returns a real decodable jpeg | ✅ pass | 0.001s |

#### Subscriber (17 tests, 0.027s)

##### FileBackedSubscriber

| Test | Outcome | Time |
|------|---------|-----:|
| Open failure throws naming the given label | ✅ pass | 0.002s |
| Write receives every envelope and the stream closes on run finished | ✅ pass | 0.001s |

##### OtrSchema

| Test | Outcome | Time |
|------|---------|-----:|
| A mixed run validates against the open test reporting schema | ✅ pass | 0.008s |

##### SubscriberRegistry

| Test | Outcome | Time |
|------|---------|-----:|
| Describe returns metadata for a valid subscriber | ✅ pass | 0.006s |
| Describe unknown key throws | ✅ pass | 0.001s |
| Describe is unavailable when a required extension is missing | ✅ pass | 0.001s |
| Describe is unavailable when the class does not exist | ✅ pass | 0.001s |
| Describe is unavailable when the class has no attribute | ✅ pass | 0.001s |
| Describe is unavailable when the class does not implement the contract | ✅ pass | 0.001s |
| All lists every configured subscriber regardless of availability | ✅ pass | 0.001s |
| Is available matches describe | ✅ pass | 0.001s |
| Has reflects what is configured | ✅ pass | 0.001s |
| Resolve constructs with validated and defaulted params | ✅ pass | 0.001s |
| Resolve throws when unavailable | ✅ pass | 0.001s |
| Resolve throws on missing required param | ✅ pass | 0.001s |
| Resolve throws on wrong param type | ✅ pass | 0.001s |
| Resolve throws on an unknown param | ✅ pass | 0.001s |

#### ProgressView (14 tests, 0.024s)

##### ProgressViewRegistry

| Test | Outcome | Time |
|------|---------|-----:|
| Describe returns metadata for a valid view | ✅ pass | 0.013s |
| Describe unknown key throws | ✅ pass | 0.001s |
| Describe is unavailable when a required extension is missing | ✅ pass | 0.001s |
| Describe is unavailable when the class does not exist | ✅ pass | 0.001s |
| Describe is unavailable when the class has no attribute | ✅ pass | 0.001s |
| Describe is unavailable when the class does not implement the contract | ✅ pass | 0.001s |
| All lists every configured view regardless of availability | ✅ pass | 0.001s |
| Is available matches describe | ✅ pass | 0.001s |
| Has reflects what is configured | ✅ pass | 0.001s |
| Resolve constructs with the given stream and validated params | ✅ pass | 0.001s |
| Resolve throws when unavailable | ✅ pass | 0.001s |
| Resolve throws on missing required param | ✅ pass | 0.001s |
| Resolve throws on wrong param type | ✅ pass | 0.001s |
| Resolve throws on an unknown param | ✅ pass | 0.001s |

#### ReportFormat (15 tests, 0.019s)

##### ReportFormatRegistry

| Test | Outcome | Time |
|------|---------|-----:|
| Describe returns metadata for a valid format | ✅ pass | 0.008s |
| Describe unknown key throws | ✅ pass | 0.001s |
| Describe is unavailable when a required extension is missing | ✅ pass | 0.001s |
| Describe is unavailable when the class does not exist | ✅ pass | 0.001s |
| Describe is unavailable when the class has no attribute | ✅ pass | 0.001s |
| Describe is unavailable when the class does not implement the contract | ✅ pass | 0.001s |
| All lists every configured format regardless of availability | ✅ pass | 0.001s |
| Is available matches describe | ✅ pass | 0.001s |
| Has reflects what is configured | ✅ pass | 0.001s |
| Resolve instantiates and applies default params | ✅ pass | 0.001s |
| Resolve throws when unavailable | ✅ pass | 0.001s |
| Resolve throws on missing required param | ✅ pass | 0.001s |
| Resolve throws on wrong param type | ✅ pass | 0.001s |
| Resolve throws on an unknown param | ✅ pass | 0.001s |
| Resolved instance can actually render | ✅ pass | 0.001s |

#### Extension (18 tests, 1.557s)

##### AssertNoDuplication

| Test | Outcome | Time |
|------|---------|-----:|
| Clean source passes | ✅ pass | 0.306s |
| A cloned body fails and is named | ✅ pass | 0.022s |
| The callers message is kept | ✅ pass | 0.015s |
| The absent tool says which package is missing | ⏭️ skip | 0.000s |
| The constraint refuses what is not a clone map | ✅ pass | 0.001s |

##### CheckExtension

| Test | Outcome | Time |
|------|---------|-----:|
| A satisfied claim passes | ✅ pass | 0.008s |
| An unsatisfied claim fails naming both operands and the detail | ✅ pass | 0.001s |
| A throwing check errors instead of crashing | ✅ pass | 0.001s |

##### CommandGate

| Test | Outcome | Time |
|------|---------|-----:|
| A zero exit is a passed check with no reason | ✅ pass | 0.048s |
| A non zero exit is a failed check naming the exit code | ✅ pass | 0.042s |
| A command past its deadline is killed and errors | ✅ pass | 1.008s |
| The event carries name and duration | ✅ pass | 0.042s |
| The builder records command gates | ✅ pass | 0.019s |
| A duplicate command label is rejected | ✅ pass | 0.001s |
| An empty argv is rejected | ✅ pass | 0.001s |

##### DuplicationCheck

| Test | Outcome | Time |
|------|---------|-----:|
| It names itself without needing the tool | ✅ pass | 0.006s |
| Asking for the check without the tool says which package is missing | ⏭️ skip | 0.000s |
| Clean source presents nothing to judge | ✅ pass | 0.005s |
| Duplication is presented as facts rather than a verdict | ✅ pass | 0.015s |
| A tolerant threshold is still the callers to set | ✅ pass | 0.015s |

#### Bridge (0.855s)

#### Laravel (8 tests, 0.827s)

##### BrowserKernelHandler

| Test | Outcome | Time |
|------|---------|-----:|
| An unbooted application is named rather than fatal | ✅ pass | 0.058s |
| The kernels response is carried back whole | ✅ pass | 0.057s |
| The response headers arrive without the ones the renderer owns | ✅ pass | 0.060s |
| The kernel is terminated after the response | ✅ pass | 0.057s |
| The request reaches the kernel intact | ✅ pass | 0.058s |

##### CrucibleServiceProvider

| Test | Outcome | Time |
|------|---------|-----:|
| The artisan test command is registered on boot | ✅ pass | 0.178s |
| A worker token arms laravels parallel testing flag | ✅ pass | 0.179s |
| A sequential run leaves the parallel flag alone | ✅ pass | 0.180s |

#### PestSnapshots (15 tests, 0.028s)

##### AutoMixedTrait

| Test | Outcome | Time |
|------|---------|-----:|
| Returns nothing when the snapshots package is not installed | ✅ pass | 0.001s |
| Returns nothing for a final class either | ✅ pass | 0.001s |

##### Functions

| Test | Outcome | Time |
|------|---------|-----:|
| Calling a proxy outside a running test throws | ✅ pass | 0.001s |
| Proxy refuses an instance that does not actually use the real trait | ✅ pass | 0.001s |
| Expect matcher refuses an instance that does not actually use the real trait | ✅ pass | 0.001s |
| To match snapshot resolves to crucibles own native matcher not spaties | ✅ pass | 0.001s |

##### SnapshotIdentityWrapper

| Test | Outcome | Time |
|------|---------|-----:|
| A class using the trait is wrapped in a subclass of it | ✅ pass | 0.007s |
| A class without the trait is left alone | ✅ pass | 0.001s |
| The trait counts wherever it is inherited | ✅ pass | 0.006s |
| The trait counts when another trait brings it | ✅ pass | 0.006s |
| Each class gets its own wrapper even sharing a parent | ✅ pass | 0.001s |
| A final class is refused rather than compiled into a fatal | ✅ pass | 0.001s |
| The generated identity resolves for a test with no dataset | ✅ pass | 0.001s |
| Each dataset row gets its own snapshot identity | ✅ pass | 0.001s |
| A named dataset row carries its label | ✅ pass | 0.001s |

#### PestLaravel (2 tests, 0.001s)

##### Functions

| Test | Outcome | Time |
|------|---------|-----:|
| Each proxy forwards to the current test instance | ✅ pass | 0.001s |
| Calling a proxy outside a running test throws | ✅ pass | 0.001s |

#### Double (83 tests, 0.639s)

##### Double

| Test | Outcome | Time |
|------|---------|-----:|
| Stub returns configured and default values | ✅ pass | 0.033s |
| Object return types yield recursive stubs | ✅ pass | 0.002s |
| With matchers select behavior per arguments | ✅ pass | 0.001s |
| Consecutive calls map and throw | ✅ pass | 0.001s |
| Abstract class double stubs all public methods | ✅ pass | 0.001s |
| Mock expectation satisfied | ✅ pass | 0.003s |
| Layered expectation keeps earlier configured return value | ✅ pass | 0.001s |
| Exceeded expectation fails at call time | ✅ pass | 0.001s |
| Unmet expectation fails verification | ✅ pass | 0.001s |
| Final classes cannot be doubled | ✅ pass | 0.001s |

##### GeneratedShapes

| Test | Outcome | Time |
|------|---------|-----:|
| Every shape generates or is recorded as not generating | ✅ pass | 0.466s |
| A by ref parameter keeps its signature and is forwarded by value | ✅ pass | 0.001s |
| A static method is refused rather than doubled | ✅ pass | 0.001s |
| A void method dispatches | ✅ pass | 0.001s |
| A tentative return type reaches the signature and the return value | ✅ pass | 0.001s |
| An object default keeps what the initializer said | ✅ pass | 0.001s |
| Defaults survive into the signature | ✅ pass | 0.001s |
| A variadic stays variadic | ✅ pass | 0.001s |

##### MockBuilder

| Test | Outcome | Time |
|------|---------|-----:|
| The original constructor runs by default | ✅ pass | 0.010s |
| Constructor args reach the original constructor | ✅ pass | 0.001s |
| Disable original constructor bypasses it | ✅ pass | 0.001s |
| Only methods leaves unlisted methods real | ✅ pass | 0.001s |
| Empty only methods doubles nothing | ✅ pass | 0.001s |
| Unknown method in only methods is a named error | ✅ pass | 0.001s |
| Only methods on an interface is a named error | ✅ pass | 0.001s |
| Configuring an undoubled method is a named error | ✅ pass | 0.001s |
| Expects on an undoubled method is a named error too | ✅ pass | 0.001s |
| Expectations on builder mocks verify | ✅ pass | 0.001s |
| The original clone runs by default and can be disabled | ✅ pass | 0.001s |
| Disabled auto return generation refuses unconfigured calls | ✅ pass | 0.001s |
| Set mock class name names the generated class | ✅ pass | 0.001s |
| A trait name is refused rather than compiled into a fatal | ✅ pass | 0.001s |
| A generated double is named by its specification not by call order | ✅ pass | 0.001s |
| Create partial mock bypasses the constructor and keeps the rest real | ✅ pass | 0.001s |
| Intersection mocks implement every interface | ✅ pass | 0.001s |
| Expectationless mocks are named and stubs are not | ✅ pass | 0.001s |
| The stub builder is the mock builder with stub spellings | ✅ pass | 0.001s |

##### MockeryMatchers

| Test | Outcome | Time |
|------|---------|-----:|
| Contains is loose and order insensitive | ✅ pass | 0.025s |
| Contains on a non array is a clean no match | ✅ pass | 0.001s |
| Has value is strict unlike contains | ✅ pass | 0.001s |
| Has key refuses non arrays | ✅ pass | 0.001s |
| Any of is strict but not any of is loose | ✅ pass | 0.002s |
| Not is strict so identity falls out for objects | ✅ pass | 0.001s |
| Subset recurses with extra keys allowed at every depth | ✅ pass | 0.002s |
| Subset loose flag and positional keys | ✅ pass | 0.001s |
| Type follows the function existence rule | ✅ pass | 0.002s |
| Pattern casts scalars and stringables | ✅ pass | 0.002s |
| Ducktype requires every real method | ✅ pass | 0.002s |
| Capture assigns by reference last call wins | ✅ pass | 0.002s |
| Capture assigns during the failed match attempt | ✅ pass | 0.001s |
| Capture composes with counts and return using | ✅ pass | 0.002s |
| Any is per argument so arity still holds | ✅ pass | 0.001s |
| On and with args predicates must return true strictly | ✅ pass | 0.002s |
| With args array form is bare with | ✅ pass | 0.001s |
| With args refuses other types in the oracles words | ✅ pass | 0.001s |
| With some of args is strict and all must be present | ✅ pass | 0.001s |
| Matchers mix with literals inside with | ✅ pass | 0.001s |
| Must be stays a named error | ✅ pass | 0.001s |

##### MockerySurface

| Test | Outcome | Time |
|------|---------|-----:|
| The pest mocking chapter shape | ✅ pass | 0.010s |
| First declared wins | ✅ pass | 0.001s |
| Count exhaustion falls through | ✅ pass | 0.001s |
| Exceeded count settles at close not call time | ✅ pass | 0.001s |
| Should not receive violation settles at close | ✅ pass | 0.001s |
| Unconfigured method is bad method call | ✅ pass | 0.001s |
| Argument mismatch is no matching expectation | ✅ pass | 0.001s |
| Mockery equality loose scalars identity objects | ✅ pass | 0.001s |
| Typed defaults match the oracle | ✅ pass | 0.001s |
| Consecutive returns repeat the last | ✅ pass | 0.001s |
| And throw with class and message | ✅ pass | 0.001s |
| Count vocabulary | ✅ pass | 0.002s |
| Between unmet settles as failure | ✅ pass | 0.001s |
| Expects defaults to once | ✅ pass | 0.001s |
| Allows is never verified | ✅ pass | 0.001s |
| Quick definitions match any arguments | ✅ pass | 0.002s |
| Quick definitions toggle makes them mocks | ✅ pass | 0.002s |
| Unknown types are declared like the oracle | ✅ pass | 0.001s |
| Constructor arguments run the original constructor | ✅ pass | 0.001s |
| Allow mocking non existent methods false refuses | ✅ pass | 0.001s |
| The global aliases are installed | ✅ pass | 0.001s |
| Ditched surface answers with named errors | ✅ pass | 0.001s |
| A mock name is a name | ✅ pass | 0.002s |
| The shapes a mock name can take | ✅ pass | 0.002s |
| A trait mock uses the trait and keeps its methods real | ✅ pass | 0.001s |

#### Mutation (41 tests, 0.583s)

##### ColdMutantExecutor

| Test | Outcome | Time |
|------|---------|-----:|
| A mutant a covering test catches is killed coldly | ✅ pass | 0.078s |
| A mutant the tests cannot see is escaped coldly | ✅ pass | 0.055s |
| A mutant no test covers is not covered | ✅ pass | 0.001s |

##### CoveringTestRunner

| Test | Outcome | Time |
|------|---------|-----:|
| The first failing covering test is the killer | ✅ pass | 0.028s |
| All covering tests surviving yields no killer | ✅ pass | 0.002s |
| Covering ids that match nothing yield no killer | ✅ pass | 0.001s |
| The cheapest covering test gets the first shot at the kill | ✅ pass | 0.002s |

##### EquivalentMarkers

| Test | Outcome | Time |
|------|---------|-----:|
| Each form covers its lines with its reason | ✅ pass | 0.008s |
| Each range starts and ends where its declaration does | ✅ pass | 0.001s |
| Generated mutants carry the reason and are never run | ✅ pass | 0.011s |
| The manuals example declares the mutants it says | ✅ pass | 0.002s |

##### MutantApplier

| Test | Outcome | Time |
|------|---------|-----:|
| A mutant the weak test cannot see is escaped | ✅ pass | 0.021s |
| A mutant the covering test catches is killed | ✅ pass | 0.015s |
| A mutant that crashes the run is errored not escaped | ✅ pass | 0.014s |
| A mutant that hangs is timed out | ✅ pass | 0.305s |
| An already loaded class is not warm applicable | ✅ pass | 0.001s |

##### MutantGenerator

| Test | Outcome | Time |
|------|---------|-----:|
| A mutant swaps exactly one operator and preserves everything else | ✅ pass | 0.003s |
| Every operator on a line becomes its own mutant | ✅ pass | 0.001s |
| Comparison and logical rules each fire | ✅ pass | 0.001s |
| Source with no operators yields no mutants | ✅ pass | 0.001s |
| The catalog is injectable | ✅ pass | 0.001s |

##### MutationJournal

| Test | Outcome | Time |
|------|---------|-----:|
| An absent journal is empty rather than an error | ✅ pass | 0.011s |
| A verdict survives being reloaded | ✅ pass | 0.001s |
| Every outcome round trips | ✅ pass | 0.001s |
| Two mutants on one line are two entries | ✅ pass | 0.001s |
| Verdicts outside the scope are left out | ✅ pass | 0.001s |
| A different judge does not match a recorded verdict | ✅ pass | 0.001s |
| A changed source invalidates its own verdict | ✅ pass | 0.001s |
| A half written last line is skipped not fatal | ✅ pass | 0.001s |
| A record missing its identity is ignored | ✅ pass | 0.001s |

##### MutationReport

| Test | Outcome | Time |
|------|---------|-----:|
| The score is detected over covered mutants | ✅ pass | 0.002s |
| All uncovered scores zero not a divide by zero | ✅ pass | 0.001s |

##### MutationRunner

| Test | Outcome | Time |
|------|---------|-----:|
| Each verdict is handed over as it lands | ✅ pass | 0.005s |
| A mutant no test covers is still handed over | ✅ pass | 0.001s |
| The runner still works with no callback | ✅ pass | 0.001s |
| A warmable mutant runs warm not cold | ✅ pass | 0.001s |
| A mutant warm cannot run falls back to cold | ✅ pass | 0.001s |
| With no warm executor everything runs cold | ✅ pass | 0.001s |
| An uncovered mutant spawns nothing | ✅ pass | 0.001s |

##### ShapeMutator

| Test | Outcome | Time |
|------|---------|-----:|
| Each string key is dropped once and the result still parses | ✅ pass | 0.003s |
| Only a string keyed element is dropped and exactly it | ✅ pass | 0.001s |

#### Coverage (46 tests, 0.450s)

##### CoverageMetadataEnforcement

| Test | Outcome | Time |
|------|---------|-----:|
| Require coverage metadata reclassifies even without a coverage run | ✅ pass | 0.002s |
| Strict check and discard over scoped windows | ✅ pass | 0.005s |

##### Coverage

| Test | Outcome | Time |
|------|---------|-----:|
| The collector filters to scope and attributes execution only | ✅ pass | 0.001s |
| Branches merge by any hit and round trip | ✅ pass | 0.001s |
| Data merges by max and totals | ✅ pass | 0.001s |
| The text report renders relative paths and totals | ✅ pass | 0.001s |
| The text report elides uncovered files unless asked | ✅ pass | 0.001s |
| The text report summary drops the rows and keeps the totals | ✅ pass | 0.001s |
| The open clover variant names the file and stamps the root | ✅ pass | 0.001s |
| The serialized php report returns the data it was given | ✅ pass | 0.001s |
| Path entries travel beside branches and tally separately | ✅ pass | 0.001s |
| The text report omits paths when none were collected | ✅ pass | 0.001s |
| The crap4j writer pairs complexity with coverage | ✅ pass | 0.002s |
| The xml report writes an index and one document per file | ✅ pass | 0.002s |
| The clover writer emits statement metrics | ✅ pass | 0.001s |
| The map derives relative edges and round trips | ✅ pass | 0.001s |
| The line map answers the mutation query and round trips | ✅ pass | 0.001s |
| The text report renders branch totals when collected | ✅ pass | 0.001s |
| The clover writer fills conditionals from branches | ✅ pass | 0.001s |
| The cobertura writer emits rates packages and condition coverage | ✅ pass | 0.001s |
| The html report writes index and annotated pages | ✅ pass | 0.002s |
| The xdebug driver collects when in coverage mode | ✅ pass | 0.000s |
| The xdebug driver collects branches when asked | ✅ pass | 0.000s |

##### CoversTargets

| Test | Outcome | Time |
|------|---------|-----:|
| No claim means identity contribution and no strays | ✅ pass | 0.001s |
| Covers class filters contribution by demoting stray hits | ✅ pass | 0.001s |
| Strays name the declaring unit | ✅ pass | 0.004s |
| Uses class allows execution but not contribution | ✅ pass | 0.001s |
| Covers nothing declares contributes nothing and is exempt from strict | ✅ pass | 0.001s |
| Unknown targets resolve to no range not an error | ✅ pass | 0.004s |
| A target that cannot load resolves to no range too | ✅ pass | 0.004s |
| Window without hits keeps denominators | ✅ pass | 0.001s |

##### ExternalCoverageArtifact

| Test | Outcome | Time |
|------|---------|-----:|
| An artifact contributes its lines and claims no test | ✅ pass | 0.001s |
| The conformance prelude writes what a child executed | ✅ pass | 0.116s |

##### MutationIndex

| Test | Outcome | Time |
|------|---------|-----:|
| Inverts the map and orders covering tests fastest first | ✅ pass | 0.001s |
| Untimed tests sort last and ties break deterministically | ✅ pass | 0.001s |
| An uncovered line or file has no tests | ✅ pass | 0.001s |

##### SourceAnalysis

| Test | Outcome | Time |
|------|---------|-----:|
| A straight line method is one | ✅ pass | 0.001s |
| Each branch adds one | ✅ pass | 0.003s |
| Ternaries count but nullable types and coalesce do not | ✅ pass | 0.003s |
| Match counts its arms and switch counts its default | ✅ pass | 0.004s |
| Reserved words used as names open no branch | ✅ pass | 0.002s |
| Boundaries survive interpolation and attributes | ✅ pass | 0.002s |
| A method reports its coverage and crap over the line map | ✅ pass | 0.001s |
| The analysis cache answers twice and notices an edit | ✅ pass | 0.138s |
| Warming parses every file it is given and skips what is not there | ✅ pass | 0.135s |
| A method with no executable line is not divided by zero | ✅ pass | 0.001s |

#### CLI (79 tests, 0.401s)

##### AnsweredOptions

| Test | Outcome | Time |
|------|---------|-----:|
| Disable coverage ignore has nothing to disable | ✅ pass | 0.001s |
| All has no configuration level selection to ignore | ✅ pass | 0.001s |
| Check version answers and exits without running anything | ✅ pass | 0.001s |
| The phpunit issue family has no issue to judge | ✅ pass | 0.002s |

##### CliOptions

| Test | Outcome | Time |
|------|---------|-----:|
| Absent options are null so configuration wins | ✅ pass | 0.001s |
| Valued options accept space and equals forms | ✅ pass | 0.001s |
| View is a valued option selecting a progress view key | ✅ pass | 0.002s |
| Repeatable options accumulate and split on commas | ✅ pass | 0.002s |
| Boolean flags parse to true not null | ✅ pass | 0.002s |
| Unknown options and stray arguments are errors | ✅ pass | 0.002s |
| Last occurrence of a valued option wins | ✅ pass | 0.002s |
| Changed takes an optional reference | ✅ pass | 0.002s |
| Bare changed never consumes the next argument | ✅ pass | 0.002s |
| An empty changed reference is an error | ✅ pass | 0.001s |
| Related accumulates | ✅ pass | 0.002s |
| Watch is a flag | ✅ pass | 0.002s |
| Retries is a numeric option | ✅ pass | 0.001s |
| Fail on flaky is a flag | ✅ pass | 0.001s |
| Flakes is a command with rounds | ✅ pass | 0.001s |
| Compat check is a command with auto fix and revert | ✅ pass | 0.001s |
| Coverage is opt in | ✅ pass | 0.001s |
| Todo listing flags parse | ✅ pass | 0.001s |
| Profile and dirty parse as flags | ✅ pass | 0.001s |
| Neither flag takes a value | ✅ pass | 0.001s |
| The specs retry spelling counts total attempts | ✅ pass | 0.001s |
| The two retry spellings are mutually exclusive | ✅ pass | 0.001s |
| Aliases are rewritten to the option they point at | ✅ pass | 0.001s |
| An alias still accepts what the option it points at accepts | ✅ pass | 0.001s |
| Do not fail on is the off half of the fail on tri state | ✅ pass | 0.002s |
| A spec spelling resolves when written with an equals | ✅ pass | 0.001s |
| A fail on switch and its negation together is an error | ✅ pass | 0.001s |
| The specs configuration switches parse as tri states | ✅ pass | 0.001s |
| Bootstrap is valued and extension repeats | ✅ pass | 0.001s |
| No coverage wins over every coverage spelling on the same command line | ✅ pass | 0.001s |
| Every stop on switch parses as a tri state | ✅ pass | 0.001s |
| The blanket off switches suppress what the same command line asked | ✅ pass | 0.001s |
| The event stream takes three independent file targets | ✅ pass | 0.001s |
| The dependency switches are a tri state and isolation is run wide | ✅ pass | 0.001s |
| The coverage surface answers one question about collecting | ✅ pass | 0.002s |
| No coverage suppresses every coverage target and the filter | ✅ pass | 0.001s |
| Include path splits on the platform separator | ✅ pass | 0.001s |
| Useless test reporting is on until turned off | ✅ pass | 0.001s |
| The coverage floor is a percentage not an integer | ✅ pass | 0.001s |
| The coverage floor collects coverage on its own | ✅ pass | 0.001s |
| A coverage floor outside zero to one hundred is an error | ✅ pass | 0.001s |
| The coverage floor and no coverage are mutually exclusive | ✅ pass | 0.001s |

##### DocumentedOptions

| Test | Outcome | Time |
|------|---------|-----:|
| Every option appears in the built in help | ✅ pass | 0.085s |
| Every option appears in the manual | ✅ pass | 0.002s |
| The manual documents no option that does not exist | ✅ pass | 0.001s |

##### PhpConfigurationCheck

| Test | Outcome | Time |
|------|---------|-----:|
| It reports the specs settings and nothing else | ✅ pass | 0.001s |
| Every result carries its own verdict | ✅ pass | 0.001s |
| Only the settings that are off produce a warning | ✅ pass | 0.001s |

##### PhpstanNeon

| Test | Outcome | Time |
|------|---------|-----:|
| A fresh file wires the extension and the project paths | ✅ pass | 0.001s |
| Wiring inserts into an existing includes section | ✅ pass | 0.001s |
| Wiring prepends a section when none exists | ✅ pass | 0.001s |
| Already wired is detected | ✅ pass | 0.001s |
| The inline list shape is refused not mangled | ✅ pass | 0.001s |
| Comments and unusual indentation survive | ✅ pass | 0.001s |
| The indent is the next entrys even on the first line | ✅ pass | 0.001s |
| A prepended section leaves the file ending in one newline | ✅ pass | 0.001s |
| An analysis configuration is written as given | ✅ pass | 0.001s |
| A fresh file leaves the include to the installer | ✅ pass | 0.001s |
| Crucible declares its extension to the installer | ✅ pass | 0.001s |

##### PostRunReport

| Test | Outcome | Time |
|------|---------|-----:|
| A scoped deprecation policy judges only its own scope | ✅ pass | 0.002s |
| The negation beats a configuration that turned the policy on | ✅ pass | 0.001s |
| Fail on all issues covers every policy and still yields to a negation | ✅ pass | 0.002s |
| An empty suite fails by default and the negation turns that off | ✅ pass | 0.002s |
| The display family names what the tally counted | ✅ pass | 0.001s |
| No display switch prints nothing | ✅ pass | 0.001s |
| Exactly the minimum passes | ✅ pass | 0.001s |
| A shortfall names the numbers | ✅ pass | 0.001s |
| No minimum is no gate | ✅ pass | 0.001s |
| Dead lines do not dilute the score | ✅ pass | 0.001s |
| The gate judges the printed percentage | ✅ pass | 0.025s |
| A floor of zero cannot be breached | ✅ pass | 0.001s |
| An empty scope is a breach | ✅ pass | 0.001s |

##### ReproducibleOutput

| Test | Outcome | Time |
|------|---------|-----:|
| The flag is off until asked for | ✅ pass | 0.001s |
| A frozen clock settles the timestamp a writer would otherwise read | ✅ pass | 0.001s |
| A wall clock writer still reports the real instant | ✅ pass | 0.001s |

#### Commands (25 tests, 0.200s)

##### CompatCheckCommand

| Test | Outcome | Time |
|------|---------|-----:|
| Fails fast when php unit is not installed | ✅ pass | 0.001s |
| An oracle that ran nothing is not agreement | ✅ pass | 0.001s |
| The candidate files are scanned for classes including pest shaped ones | ✅ pass | 0.001s |
| Revert restores files from an existing manifest | ✅ pass | 0.002s |
| Revert with nothing to revert is still successful | ✅ pass | 0.001s |

##### CompletionCommand

| Test | Outcome | Time |
|------|---------|-----:|
| Each shell offers every option the parser accepts | ✅ pass | 0.005s |
| The script is only script | ✅ pass | 0.002s |
| An unknown shell is refused with the list | ✅ pass | 0.001s |

##### ExtensionsCommand

| Test | Outcome | Time |
|------|---------|-----:|
| List shows all three kinds with a kind column | ✅ pass | 0.006s |
| List json tags each entry with its kind | ✅ pass | 0.002s |
| Detail finds a report format by key | ✅ pass | 0.002s |
| Detail finds a subscriber by key | ✅ pass | 0.002s |
| Detail finds a progress view by key | ✅ pass | 0.002s |
| Detail unknown key errors across all registries | ✅ pass | 0.002s |
| Preview without key errors | ✅ pass | 0.002s |
| Preview without a key asks and previews the answer | ✅ pass | 0.016s |
| Preview report format writes the rendered document | ✅ pass | 0.009s |
| Preview subscriber writes a real well formed j unit report | ✅ pass | 0.003s |
| Preview progress view writes real team city service messages | ✅ pass | 0.002s |

##### InitCommand

| Test | Outcome | Time |
|------|---------|-----:|
| Non interactive terminal writes the prior static template unchanged | ✅ pass | 0.001s |
| Interactive prompts customize the generated config | ✅ pass | 0.060s |
| Declined overwrite keeps the existing file | ✅ pass | 0.006s |
| Confirmed overwrite replaces the file | ✅ pass | 0.017s |
| Unsafe characters are rejected until corrected | ✅ pass | 0.053s |
| Existing phpunit xml is converted instead of prompting | ✅ pass | 0.001s |

#### Console (0.287s)

#### Components (19 tests, 0.155s)

##### SelectPrompt

| Test | Outcome | Time |
|------|---------|-----:|
| The list is drawn with every option and the hint | ✅ pass | 0.007s |
| One option at a time carries the marker | ✅ pass | 0.007s |
| The arrow keys choose and enter answers | ✅ pass | 0.014s |
| The list wraps at both ends | ✅ pass | 0.030s |
| Without a default it refuses to answer for a script | ✅ pass | 0.001s |
| A default is an answer a script can use | ✅ pass | 0.001s |

##### Splash

| Test | Outcome | Time |
|------|---------|-----:|
| A non interactive terminal gets one static line | ✅ pass | 0.001s |
| An interactive terminal sweeps and settles | ✅ pass | 0.016s |
| Fewer sweeps is proportionally fewer frames | ✅ pass | 0.009s |
| A frame carries all three states | ✅ pass | 0.016s |
| It settles with the whole wordmark lit | ✅ pass | 0.001s |
| A classic terminal gets no truecolor sequences | ✅ pass | 0.028s |
| A single character wordmark terminates | ✅ pass | 0.001s |
| An empty wordmark writes nothing | ✅ pass | 0.001s |
| The suffix follows the wordmark on every frame | ✅ pass | 0.017s |
| The sweep bounces on a single cell per tick | ✅ pass | 0.003s |
| A single cell sweep stays put | ✅ pass | 0.001s |
| Every frame carries the suffix | ✅ pass | 0.001s |
| A wide character is one cell | ✅ pass | 0.001s |

#### Output (22 tests, 0.059s)

##### Help

| Test | Outcome | Time |
|------|---------|-----:|
| Descriptions share one column | ✅ pass | 0.001s |
| A term too wide for the column takes its own line | ✅ pass | 0.001s |
| A long description wraps into the same column | ✅ pass | 0.002s |
| A list nested under an option is laid out on its own | ✅ pass | 0.002s |
| An unbreakable description is not split mid word | ✅ pass | 0.001s |
| Colour is worn only when the terminal can render it | ✅ pass | 0.001s |
| Prose is untouched | ✅ pass | 0.001s |

##### Markdown

| Test | Outcome | Time |
|------|---------|-----:|
| Strips bold markers | ✅ pass | 0.001s |
| Strips inline code and italics | ✅ pass | 0.001s |
| Headings | ✅ pass | 0.001s |
| Bullet list | ✅ pass | 0.001s |
| Collects links as numbered references | ✅ pass | 0.001s |
| External and local links are both collected in order | ✅ pass | 0.001s |
| Wraps long paragraphs | ✅ pass | 0.001s |
| Bold span crossing a hard wrapped source line is still parsed | ✅ pass | 0.001s |
| Bullet continuation line joins the same item | ✅ pass | 0.001s |
| Blank line ends a bullet continuation | ✅ pass | 0.001s |
| Table renders as a bordered grid with a header row | ✅ pass | 0.001s |
| Table cells keep followable link references | ✅ pass | 0.001s |

##### TextPdf

| Test | Outcome | Time |
|------|---------|-----:|
| It produces a readable pdf | ✅ pass | 0.001s |
| Long text is paginated | ✅ pass | 0.034s |
| The manual itself renders | ✅ pass | 0.002s |

#### Support (15 tests, 0.051s)

##### Str

| Test | Outcome | Time |
|------|---------|-----:|
| Every width range edge holds on both sides | ✅ pass | 0.002s |
| An emoji presentation sequence is one emoji wide | ✅ pass | 0.001s |
| Dingbats below the emoji range measure one column | ✅ pass | 0.001s |
| Char width of nothing is zero | ✅ pass | 0.001s |
| Width counts columns not characters | ✅ pass | 0.001s |
| Width ignores ansi sequences | ✅ pass | 0.001s |
| Length counts characters and not columns | ✅ pass | 0.001s |
| Truncate keeps what fits and marks what it cut | ✅ pass | 0.001s |
| Padding measures columns not bytes | ✅ pass | 0.001s |
| Padding at or over the width is left alone | ✅ pass | 0.001s |
| Wrap breaks on words and keeps paragraphs | ✅ pass | 0.001s |
| Wrap hard breaks a word too long to fit | ✅ pass | 0.001s |
| Wrap with no room returns the input whole | ✅ pass | 0.001s |
| Substr counts characters | ✅ pass | 0.001s |
| Width stays correct once the memo is full | ✅ pass | 0.041s |

#### Runtime (5 tests, 0.016s)

##### ModalPresenter

| Test | Outcome | Time |
|------|---------|-----:|
| It takes the alternate screen and hands it back | ✅ pass | 0.007s |
| The surface is taken only once | ✅ pass | 0.001s |
| The dialog is boxed and centred | ✅ pass | 0.007s |
| It draws its own frame so prompts render bare | ✅ pass | 0.001s |
| The dialog never fills the screen edge to edge | ✅ pass | 0.001s |

#### Terminal (10 tests, 0.006s)

##### Capabilities

| Test | Outcome | Time |
|------|---------|-----:|
| A terminal gets both | ✅ pass | 0.001s |
| A pipe gets neither | ✅ pass | 0.001s |
| Continuous integration keeps colour and loses animation | ✅ pass | 0.001s |
| A false ci marker is not continuous integration | ✅ pass | 0.001s |
| A dumb terminal gets neither despite being a tty | ✅ pass | 0.001s |
| An empty term is treated as dumb | ✅ pass | 0.001s |
| A known term is fine | ✅ pass | 0.001s |
| No color beats force color | ✅ pass | 0.001s |
| Force color paints a pipe | ✅ pass | 0.001s |
| The overrides win and reset together | ✅ pass | 0.001s |

#### Impact (58 tests, 0.216s)

##### ChangedFiles

| Test | Outcome | Time |
|------|---------|-----:|
| Modified untracked and deleted files are reported | ✅ pass | 0.018s |
| A clean tree reports nothing | ✅ pass | 0.011s |
| An unknown reference is an error | ✅ pass | 0.009s |
| Outside a repository is an error | ✅ pass | 0.008s |

##### DependencyGraph

| Test | Outcome | Time |
|------|---------|-----:|
| The closure follows references transitively | ✅ pass | 0.016s |
| An island reaches only itself | ✅ pass | 0.001s |
| Vendor files are never graph nodes | ✅ pass | 0.016s |
| Vendor is excluded by path segment not only at the root | ✅ pass | 0.003s |
| Observed edges apply one hop from the root only | ✅ pass | 0.002s |
| Pest family files depend on the suite configuration above them | ✅ pass | 0.001s |

##### DependencyIndex

| Test | Outcome | Time |
|------|---------|-----:|
| A warm index produces the identical closure | ✅ pass | 0.060s |
| A changed file is not replayed from the index | ✅ pass | 0.001s |
| A different configuration lands on a different index | ✅ pass | 0.001s |
| A suite configuration appearing changes the fingerprint | ✅ pass | 0.001s |
| An index survives the checkout moving to another path | ✅ pass | 0.001s |
| The fingerprint does not depend on where the project sits | ✅ pass | 0.001s |
| An entry reaching outside the project is not stored | ✅ pass | 0.001s |
| An entry wholly inside the project is still stored | ✅ pass | 0.001s |

##### ImpactFingerprint

| Test | Outcome | Time |
|------|---------|-----:|
| Adding a suite configuration changes the fingerprint | ✅ pass | 0.005s |
| The same tree fingerprints the same | ✅ pass | 0.001s |
| Configuration above the file counts too | ✅ pass | 0.001s |

##### ImpactSelection

| Test | Outcome | Time |
|------|---------|-----:|
| A change selects the groups whose closure reaches it | ✅ pass | 0.017s |
| A changed test file selects itself | ✅ pass | 0.002s |
| An untouched graph selects nothing | ✅ pass | 0.003s |
| A change a vitest suite answers for is not called unaccounted for | ✅ pass | 0.001s |
| A change no test reaches says so rather than going quiet | ✅ pass | 0.002s |
| Deletions widen to the full suite | ✅ pass | 0.001s |
| Composer changes widen to the full suite | ✅ pass | 0.001s |
| A javascript dependency bump widens too | ✅ pass | 0.001s |
| Environment files widen to the full suite | ✅ pass | 0.001s |
| A non php change is reported in the notes | ✅ pass | 0.001s |
| A rule selects its groups for an unreachable file | ✅ pass | 0.002s |
| A rule matches templates that end in php | ✅ pass | 0.001s |
| Rules only widen never narrow | ✅ pass | 0.002s |
| A group selected by both sources is not duplicated | ✅ pass | 0.002s |
| A rule match is not counted as an ignored change | ✅ pass | 0.001s |
| A rule for a group no test carries is reported | ✅ pass | 0.001s |
| A glob pattern matches across directories | ✅ pass | 0.001s |
| A change matching no rule selects nothing | ✅ pass | 0.001s |

##### ReferenceScanner

| Test | Outcome | Time |
|------|---------|-----:|
| Use imports resolve fully | ✅ pass | 0.003s |
| Aliases resolve to the imported name | ✅ pass | 0.001s |
| Group use expands the prefix | ✅ pass | 0.001s |
| Unimported names resolve against the namespace | ✅ pass | 0.001s |
| Fully qualified names pass through | ✅ pass | 0.001s |
| Qualified names join the namespace | ✅ pass | 0.001s |
| Extends implements and attributes are references | ✅ pass | 0.001s |
| Declarations are not references | ✅ pass | 0.001s |
| Member access is not a reference | ✅ pass | 0.001s |
| Lowercase identifiers are not candidates | ✅ pass | 0.001s |
| Global fallback only without a namespace | ✅ pass | 0.001s |
| Use function imports are skipped | ✅ pass | 0.001s |
| Closure capture lists are not imports | ✅ pass | 0.001s |
| Trait use inside a class is a reference | ✅ pass | 0.001s |

##### VitestImpact

| Test | Outcome | Time |
|------|---------|-----:|
| A change under a suite narrows it to that related file | ✅ pass | 0.005s |
| A suite with no js change is dropped but named | ✅ pass | 0.001s |
| Deletions widen every suite to a full run | ✅ pass | 0.001s |
| No configured suites yields nothing | ✅ pass | 0.001s |
| Each suite is scoped independently | ✅ pass | 0.001s |

#### Watch (30 tests, 0.151s)

##### FileWatcher

| Test | Outcome | Time |
|------|---------|-----:|
| Vendor node modules and hidden directories are not watched | ✅ pass | 0.006s |
| Modifications additions and deletions are diffed | ✅ pass | 0.001s |
| A touch alone is a change | ✅ pass | 0.001s |
| Explicit files are watched too | ✅ pass | 0.001s |

##### RetriggerEndpoint

| Test | Outcome | Time |
|------|---------|-----:|
| A pushed change set is accepted and handed over once | ✅ pass | 0.007s |
| The token is required | ✅ pass | 0.001s |
| A missing token is refused | ✅ pass | 0.001s |
| Only post is accepted | ✅ pass | 0.001s |
| A malformed body is refused rather than guessed | ✅ pass | 0.001s |
| Non string entries are dropped not coerced | ✅ pass | 0.001s |
| The payload carries paths and nothing command shaped | ✅ pass | 0.001s |

##### RetriggerListener

| Test | Outcome | Time |
|------|---------|-----:|
| The hot file is written while listening and removed on close | ✅ pass | 0.012s |
| A real push over the socket reaches the loop | ✅ pass | 0.001s |
| A push with the wrong token is refused over the socket | ✅ pass | 0.001s |
| The shipped node producer pushes through the documented contract | ✅ pass | 0.071s |
| A producer finding no hot file does nothing | ✅ pass | 0.032s |

##### WatchSession

| Test | Outcome | Time |
|------|---------|-----:|
| A green session runs the affected files | ✅ pass | 0.007s |
| Deletions widen to the full suite | ✅ pass | 0.001s |
| Non php changes widen to the full suite | ✅ pass | 0.001s |
| A file a declared rule names runs related not full | ✅ pass | 0.001s |
| A file no rule names still widens | ✅ pass | 0.001s |
| A rule does not rescue a deletion | ✅ pass | 0.001s |
| A js change under a vitest suite runs related not full | ✅ pass | 0.001s |
| A non php change outside every vitest suite still widens to full | ✅ pass | 0.001s |
| The failed set is sticky across changes | ✅ pass | 0.001s |
| A green partial run after red earns one full confirmation | ✅ pass | 0.001s |
| A green partial run without prior failures needs no confirmation | ✅ pass | 0.001s |
| A still red run waits instead of looping | ✅ pass | 0.001s |
| The failed only run is null when green | ✅ pass | 0.001s |
| The failed only run targets exactly the failed files | ✅ pass | 0.001s |

#### Compat/Migration (46 tests, 0.107s)

##### CompositeEqualsPattern

| Test | Outcome | Time |
|------|---------|-----:|
| Real introspection processor shape drops coupled keys keeps the rest | ✅ pass | 0.037s |
| No backing array assignment is not auto fixed | ✅ pass | 0.001s |
| Non variable argument is not auto fixed | ✅ pass | 0.001s |
| A third argument is not auto fixed | ✅ pass | 0.001s |
| Every key coupled is not auto fixed | ✅ pass | 0.001s |
| Long array syntax is not auto fixed | ✅ pass | 0.001s |
| Static call prefix is preserved on every generated statement | ✅ pass | 0.037s |
| Preview does not touch the source | ✅ pass | 0.001s |

##### CrucibleRun

| Test | Outcome | Time |
|------|---------|-----:|
| The child carries the pest vocabulary prelude | ✅ pass | 0.001s |
| Keeps only test finish events keyed by id | ✅ pass | 0.001s |
| Malformed lines are ignored | ✅ pass | 0.001s |
| No events file yields no outcomes | ✅ pass | 0.001s |

##### FixManifest

| Test | Outcome | Time |
|------|---------|-----:|
| Backup then revert restores original content | ✅ pass | 0.001s |
| Revert clears the manifest | ✅ pass | 0.001s |
| A second backup of the same file is a no op | ✅ pass | 0.001s |
| Multiple files revert together | ✅ pass | 0.001s |
| Empty manifest has nothing to revert | ✅ pass | 0.001s |

##### OracleRun

| Test | Outcome | Time |
|------|---------|-----:|
| Keys by relative file path and method not method alone | ✅ pass | 0.001s |
| Outcome classification | ✅ pass | 0.001s |
| Dataset suffix is appended to the key | ✅ pass | 0.001s |
| File outside the working directory stays absolute | ✅ pass | 0.001s |
| Pest reports the id itself in the file attribute | ✅ pass | 0.001s |
| A positional pest dataset is counted and a named one is read | ✅ pass | 0.001s |
| A classic class inside a pest run is reported unmapped not guessed | ✅ pass | 0.001s |
| The oracle binary is pest wherever pest is installed | ✅ pass | 0.001s |

##### OutcomeDiff

| Test | Outcome | Time |
|------|---------|-----:|
| Flags only oracle pass crucible fail or error | ✅ pass | 0.001s |
| No drift when everything agrees | ✅ pass | 0.001s |
| Oracle non pass outcomes are never candidates regardless of crucible side | ✅ pass | 0.001s |
| A test the oracle ran and crucible did not is reported missing | ✅ pass | 0.001s |
| An empty crucible run is every oracle pass missing rather than no drift | ✅ pass | 0.001s |
| A test the oracle did not pass is not owed an outcome | ✅ pass | 0.001s |
| Nothing is missing when crucible answered every oracle pass | ✅ pass | 0.001s |

##### PhpUnitEventLog

| Test | Outcome | Time |
|------|---------|-----:|
| It reads the class based rows and leaves pests own to junit | ✅ pass | 0.001s |
| The verdict is by precedence not by arrival | ✅ pass | 0.001s |
| A class is placed by the file that declares it and never by resemblance | ✅ pass | 0.001s |

##### SourceRewriter

| Test | Outcome | Time |
|------|---------|-----:|
| Locate method finds the declaration to closing brace span | ✅ pass | 0.001s |
| Locate method ignores a call to the same name elsewhere | ✅ pass | 0.001s |
| Locate method returns null for an abstract method | ✅ pass | 0.001s |
| Locate method returns null when not found | ✅ pass | 0.001s |
| Vendor path assertion on an array indexed higher frame weakens to a string check | ✅ pass | 0.001s |
| Vendor path assertion with a frame number prefix on a higher frame keeps only the frame marker | ✅ pass | 0.001s |
| Vendor path assertion becomes a wildcard regex | ✅ pass | 0.001s |
| No equivalent filename becomes a structural frame check | ✅ pass | 0.001s |
| Unrelated assertion is a byte exact no op | ✅ pass | 0.001s |
| Out of range line is ignored | ✅ pass | 0.001s |
| Preview does not touch the source | ✅ pass | 0.001s |

#### Vitest (9 tests, 0.103s)

##### VitestReport

| Test | Outcome | Time |
|------|---------|-----:|
| Translates each assertion result to a test finished | ✅ pass | 0.007s |
| A failed test carries the failure message | ✅ pass | 0.001s |
| Todo maps to incomplete and other statuses to skipped | ✅ pass | 0.001s |
| A file outside the base keeps its absolute path so it round trips through related | ✅ pass | 0.001s |
| Malformed entries are skipped not fatal | ✅ pass | 0.001s |

##### VitestRunner

| Test | Outcome | Time |
|------|---------|-----:|
| An unfiltered suite runs whole and reports every skip | ✅ pass | 0.049s |
| A filter becomes the test name pattern and its leftovers are not reported | ✅ pass | 0.043s |
| A substring filter keeps its wildcard and escapes the rest | ✅ pass | 0.001s |
| A regular expression filter passes its body through | ✅ pass | 0.001s |

#### Snapshot (37 tests, 0.066s)

##### InlineSnapshot

| Test | Outcome | Time |
|------|---------|-----:|
| A matching recorded value passes without queuing a rewrite | ✅ pass | 0.007s |
| A mismatch fails when not updating | ✅ pass | 0.001s |
| An absent value fails naming the flag | ✅ pass | 0.001s |
| Recording when rewriting is forbidden fails naming the constraint | ✅ pass | 0.001s |
| Recording sequentially queues the rewrite | ✅ pass | 0.001s |
| A scalar inline snapshot compares live | ✅ pass | 0.001s |
| An array inline snapshot compares live | ✅ pass | 0.001s |

##### InlineSnapshotWriter

| Test | Outcome | Time |
|------|---------|-----:|
| Records into an empty call | ✅ pass | 0.003s |
| Replaces an existing literal | ✅ pass | 0.001s |
| The phpunit spelling preserves the value and appends the snapshot | ✅ pass | 0.001s |
| A multi line value becomes a nowdoc | ✅ pass | 0.001s |
| An unpreserved chain after the call survives | ✅ pass | 0.001s |
| No matching call leaves the source byte exact | ✅ pass | 0.001s |
| Single quote escaping round trips | ✅ pass | 0.001s |
| The nowdoc marker avoids collision with content | ✅ pass | 0.001s |
| Flush applies every queued edit bottom up | ✅ pass | 0.001s |

##### SnapshotDialect.crucible

| Test | Outcome | Time |
|------|---------|-----:|
| A receipt keeps its shape | ✅ pass | 0.002s |
| An inline snapshot compares against the value recorded in the call | ✅ pass | 0.001s |
| Negating an inline snapshot is refused | ✅ pass | 0.001s |
| Several snapshots number themselves | ✅ pass | 0.001s |

##### SnapshotPruner

| Test | Outcome | Time |
|------|---------|-----:|
| A complete run prunes unvisited entries | ✅ pass | 0.009s |
| An incomplete run prunes nothing | ✅ pass | 0.001s |
| A failed test shields its whole snapshot file | ✅ pass | 0.001s |
| A fully obsolete file is deleted with its empty directories | ✅ pass | 0.001s |
| A pruned screenshot entry takes its images along | ✅ pass | 0.001s |

##### Snapshot

| Test | Outcome | Time |
|------|---------|-----:|
| The format round trips hostile content | ✅ pass | 0.009s |
| Editor trimmed blank lines still parse | ✅ pass | 0.001s |
| Missing snapshot fails and names the flag | ✅ pass | 0.002s |
| Update records then a normal run matches | ✅ pass | 0.002s |
| A changed value fails with the stored expectation | ✅ pass | 0.002s |
| The screenshot flavor stores the reference and renders a visual diff | ✅ pass | 0.003s |
| Update runs report created and updated counts | ✅ pass | 0.003s |
| Visited keys ride the finish event | ✅ pass | 0.002s |
| A filtered update keeps unvisited keys | ✅ pass | 0.002s |
| Named and counted snapshots coexist | ✅ pass | 0.002s |
| Outside the runner snapshots refuse loudly | ✅ pass | 0.001s |
| The dogfood snapshot matches | ✅ pass | 0.001s |

#### Event (17 tests, 0.039s)

##### Emitter

| Test | Outcome | Time |
|------|---------|-----:|
| Stamps gapless one based sequence and clock time | ✅ pass | 0.005s |
| Delivers to listeners in subscription order | ✅ pass | 0.001s |

##### EventPayload

| Test | Outcome | Time |
|------|---------|-----:|
| Optional fields are omitted not null | ✅ pass | 0.007s |
| Retry attempt and skip reason appear when set | ✅ pass | 0.001s |
| Blocked appears only when set | ✅ pass | 0.001s |
| Untested is a subset of skipped not an extra outcome | ✅ pass | 0.003s |
| Untested rides run finished as an additive field | ✅ pass | 0.002s |
| Run summary plus sums every field for the vitest fold | ✅ pass | 0.001s |
| Failure payload omits absent parts | ✅ pass | 0.002s |
| Run summary counts and verdict | ✅ pass | 0.001s |

##### EventTextWriter

| Test | Outcome | Time |
|------|---------|-----:|
| Terse form is sequence and name only | ✅ pass | 0.005s |
| Verbose form keeps the payload fields | ✅ pass | 0.001s |
| Telemetry prefixes each line with elapsed time and peak memory | ✅ pass | 0.001s |

##### NdjsonStream

| Test | Outcome | Time |
|------|---------|-----:|
| Miniature run produces the exact golden stream | ✅ pass | 0.008s |
| Incomplete carries its origin and skipped does not | ✅ pass | 0.001s |
| Output chunk concatenation is exact | ✅ pass | 0.001s |
| Invalid utf8 in chunks is substituted not fatal | ✅ pass | 0.001s |

#### Assert (40 tests, 0.028s)

##### Assert

| Test | Outcome | Time |
|------|---------|-----:|
| Identity and counting | ✅ pass | 0.001s |
| Same on strings carries structured diff | ✅ pass | 0.001s |
| Equality families | ✅ pass | 0.001s |
| Boolean null and emptiness | ✅ pass | 0.001s |
| Counts and sizes | ✅ pass | 0.001s |
| Comparisons | ✅ pass | 0.001s |
| Iterable families | ✅ pass | 0.001s |
| String families | ✅ pass | 0.001s |
| Object and type families | ✅ pass | 0.001s |
| Filesystem families | ✅ pass | 0.001s |
| Fail throws and prepends custom messages | ✅ pass | 0.001s |

##### AssertTranche

| Test | Outcome | Time |
|------|---------|-----:|
| Case and line ending insensitive equality | ✅ pass | 0.001s |
| Float specials | ✅ pass | 0.001s |
| Object equals uses the declared protocol | ✅ pass | 0.001s |
| String matches format | ✅ pass | 0.001s |
| File content equality | ✅ pass | 0.001s |
| Missing file is a failure not an error | ✅ pass | 0.000s |
| Json comparisons | ✅ pass | 0.001s |
| Readability and writability | ✅ pass | 0.001s |

##### Differ

| Test | Outcome | Time |
|------|---------|-----:|
| Marks removals additions and context | ✅ pass | 0.001s |
| Pure addition and removal | ✅ pass | 0.001s |
| Context collapses the unchanged runs around each change | ✅ pass | 0.001s |
| Without context every unchanged line survives | ✅ pass | 0.001s |

##### EqualitySemantics

| Test | Outcome | Time |
|------|---------|-----:|
| Numeric juggling between number and numeric string | ✅ pass | 0.001s |
| Two strings never juggle numerically | ✅ pass | 0.001s |
| Nan is never equal | ✅ pass | 0.001s |
| Delta applies to numbers and recurses into arrays | ✅ pass | 0.001s |
| Arrays compare by keys order insensitive | ✅ pass | 0.001s |
| Canonicalize compares lists as multisets | ✅ pass | 0.001s |
| Date times compare by instant | ✅ pass | 0.001s |
| Objects compare by class and properties recursively | ✅ pass | 0.001s |
| Cyclic object graphs do not recurse forever | ✅ pass | 0.001s |
| A stringable object equals its string form | ✅ pass | 0.001s |
| A non stringable object is never equal to a string | ✅ pass | 0.001s |

##### Exporter

| Test | Outcome | Time |
|------|---------|-----:|
| Scalars | ✅ pass | 0.001s |
| Arrays are multiline and nested | ✅ pass | 0.001s |
| Objects export class and properties | ✅ pass | 0.001s |
| Object recursion is guarded | ✅ pass | 0.001s |
| Enums export as class and case | ✅ pass | 0.001s |
| Describe is short for compound values | ✅ pass | 0.001s |

#### Configuration (29 tests, 0.024s)

##### Builder

| Test | Outcome | Time |
|------|---------|-----:|
| Defaults match the phpunit spec | ✅ pass | 0.001s |
| Maps the phpunit xml core surface | ✅ pass | 0.001s |
| Strict enables every fail on flag | ✅ pass | 0.001s |
| Rejects duplicate test suite names | ✅ pass | 0.001s |
| Report format registers a class string and params | ✅ pass | 0.001s |
| Report format calling twice with the same key overrides rather than throws | ✅ pass | 0.001s |
| Subscriber registers a class string and params | ✅ pass | 0.001s |
| Subscriber calling twice with the same key overrides rather than throws | ✅ pass | 0.001s |

##### Loader

| Test | Outcome | Time |
|------|---------|-----:|
| Loads a configuration file that returns a builder | ✅ pass | 0.001s |
| Falls back to dist file | ✅ pass | 0.001s |
| Explicit path wins over default file names | ✅ pass | 0.001s |
| Rejects a missing explicit path | ✅ pass | 0.001s |
| Rejects a directory without configuration | ✅ pass | 0.001s |
| Rejects a configuration file with a wrong return type | ✅ pass | 0.001s |
| A configuration that throws is reported not fatal | ✅ pass | 0.001s |
| A configuration throwing a string code is reported not a type error | ✅ pass | 0.001s |
| Exists checks default file names | ✅ pass | 0.001s |

##### Quirk

| Test | Outcome | Time |
|------|---------|-----:|
| No quirk is declared | ✅ pass | 0.001s |
| A removed quirk is not accepted as a name | ✅ pass | 0.001s |
| The configuration still carries an empty list | ✅ pass | 0.001s |
| The falsy zero is not a special case but is empty | ✅ pass | 0.001s |
| The hostname trap is the same emptiness one layer down | ✅ pass | 0.001s |
| The cast is the default and not an opt in | ✅ pass | 0.001s |
| Everything the incumbent casts is cast | ✅ pass | 0.001s |
| The refusal is not a verdict and never was quirk gated | ✅ pass | 0.001s |

##### XmlMigrator

| Test | Outcome | Time |
|------|---------|-----:|
| Migrated configuration loads with the right typed values | ✅ pass | 0.002s |
| Everything without a crucible equivalent is named in the notes | ✅ pass | 0.001s |
| Defaults are not restated in the generated code | ✅ pass | 0.001s |
| Unparseable xml throws | ✅ pass | 0.001s |

#### Flakiness (14 tests, 0.023s)

##### FailureOutsideDiff

| Test | Outcome | Time |
|------|---------|-----:|
| A failure that executed no changed file is a suspect | ✅ pass | 0.008s |
| A failure that executed a changed file is never a suspect | ✅ pass | 0.001s |
| A failing test whose own file changed is never a suspect | ✅ pass | 0.001s |
| A changed declaring file of another test does not suppress the check | ✅ pass | 0.001s |
| Unobservable changed code silences the check entirely | ✅ pass | 0.001s |
| A test only diff produces no hint | ✅ pass | 0.001s |
| A failure unknown to the map is skipped | ✅ pass | 0.001s |
| Empty inputs are silence | ✅ pass | 0.001s |
| A whole file scope entry matches exactly | ✅ pass | 0.001s |

##### OrderDependencyHunter

| Test | Outcome | Time |
|------|---------|-----:|
| A seed reproduced failure that passes alone is order dependent | ✅ pass | 0.007s |
| A failure the seed cannot reproduce is non deterministic | ✅ pass | 0.001s |
| A failure that fails alone is broken not flaky | ✅ pass | 0.001s |
| Baseline failures are named and excluded from the hunt | ✅ pass | 0.001s |
| A clean suite reports clean | ✅ pass | 0.001s |

#### Framework (11 tests, 0.021s)

##### LifecycleCompatibility

| Test | Outcome | Time |
|------|---------|-----:|
| A traits before reset runs ahead of set up | ✅ pass | 0.013s |
| The plan places each template at priority zero | ✅ pass | 0.001s |
| An attribute on a template method does not run it twice | ✅ pass | 0.001s |
| An error from the test passes through transform exception | ✅ pass | 0.002s |
| An error from set up passes through transform exception | ✅ pass | 0.001s |
| A failure is an outcome and is not transformed | ✅ pass | 0.001s |
| An expected exception is not transformed | ✅ pass | 0.001s |
| The incumbents logical not is aliased | ✅ pass | 0.001s |
| A framework constraint fails in the incumbents sentence | ✅ pass | 0.001s |
| Its negation negates the wording and not the data | ✅ pass | 0.001s |
| The negation passes | ✅ pass | 0.001s |

#### Polyfill (0.019s)

#### Php84 (16 tests, 0.013s)

##### ArrayFunctions

| Test | Outcome | Time |
|------|---------|-----:|
| Any is false on an empty array | ✅ pass | 0.005s |
| Any is false when no element matches | ✅ pass | 0.001s |
| Any is true when an element matches | ✅ pass | 0.001s |
| Any passes the key to the callback | ✅ pass | 0.001s |
| All is true on an empty array | ✅ pass | 0.001s |
| All is true when every element matches | ✅ pass | 0.001s |
| All is false when any element fails | ✅ pass | 0.001s |
| All passes the key to the callback | ✅ pass | 0.001s |
| Find returns null on an empty array | ✅ pass | 0.001s |
| Find returns null when no element matches | ✅ pass | 0.001s |
| Find returns the first matching value | ✅ pass | 0.001s |
| Find passes the key to the callback | ✅ pass | 0.001s |
| Find key returns null on an empty array | ✅ pass | 0.001s |
| Find key returns null when no element matches | ✅ pass | 0.001s |
| Find key returns the first matching key | ✅ pass | 0.001s |
| Find key short circuits on the first match | ✅ pass | 0.001s |

#### Php85 (8 tests, 0.006s)

##### ArrayFunctions

| Test | Outcome | Time |
|------|---------|-----:|
| First returns null on an empty array | ✅ pass | 0.002s |
| First returns the first value of a list array | ✅ pass | 0.001s |
| First returns the first value of an associative array | ✅ pass | 0.001s |
| First returns null when the first value is itself null | ✅ pass | 0.001s |
| Last returns null on an empty array | ✅ pass | 0.001s |
| Last returns the last value of a list array | ✅ pass | 0.001s |
| Last returns the last value of an associative array | ✅ pass | 0.001s |
| Last returns null when the last value is itself null | ✅ pass | 0.001s |

#### Isolation (6 tests, 0.010s)

##### GlobalStateExport

| Test | Outcome | Time |
|------|---------|-----:|
| A global survives the round trip through the manifest | ✅ pass | 0.007s |
| A null global round trips as a value rather than as absent | ✅ pass | 0.001s |
| What no serializer can carry is skipped by name not fatal | ✅ pass | 0.001s |
| Superglobals are left to the process they describe | ✅ pass | 0.001s |
| Only user constants travel and restoring never redefines | ✅ pass | 0.001s |
| Garbage from the manifest is ignored rather than trusted | ✅ pass | 0.001s |

#### Metadata (5 tests, 0.009s)

##### MetadataParser

| Test | Outcome | Time |
|------|---------|-----:|
| Collects class level attributes including inherited | ✅ pass | 0.004s |
| Collects method attributes in declaration order | ✅ pass | 0.002s |
| Method metadata precedes class metadata in merged view | ✅ pass | 0.001s |
| Foreign attributes are ignored | ✅ pass | 0.001s |
| Programmatic construction for dialect frontends | ✅ pass | 0.001s |

#### Generated (7 tests, 0.009s)

##### GeneratedCode

| Test | Outcome | Time |
|------|---------|-----:|
| It compiles and hands back what the source returns | ✅ pass | 0.004s |
| Source that does not parse names what it was for and shows it | ✅ pass | 0.001s |
| Recording writes the source with what it was for | ✅ pass | 0.001s |
| The same shape twice is one recorded file | ✅ pass | 0.001s |
| Recording stops when the scope ends | ✅ pass | 0.001s |
| Recording stops even when the work throws | ✅ pass | 0.001s |
| A failure inside the generated code is not a generation failure | ✅ pass | 0.001s |

#### Filesystem (8 tests, 0.007s)

##### WorkingDirectory

| Test | Outcome | Time |
|------|---------|-----:|
| An empty path is refused at construction | ✅ pass | 0.003s |
| The path is kept verbatim | ✅ pass | 0.001s |
| Relative paths resolve against the directory | ✅ pass | 0.001s |
| An absolute path is returned untouched | ✅ pass | 0.001s |
| The ugly shapes are preserved rather than fixed | ✅ pass | 0.001s |
| Current reads the process directory | ✅ pass | 0.001s |
| Two directories are equal by path | ✅ pass | 0.001s |
| A path inside the directory is named from it | ✅ pass | 0.001s |

#### Test (3 tests, 0.003s)

##### TestId

| Test | Outcome | Time |
|------|---------|-----:|
| String form is file name and optional dataset | ✅ pass | 0.002s |
| Hash is stable and discriminates | ✅ pass | 0.001s |
| Equality | ✅ pass | 0.001s |

#### examples (1.633s)

#### 07-type-tests (2 tests, 1.505s)

##### ids.types

| Test | Outcome | Time |
|------|---------|-----:|
| Line 21: list<int> | ✅ pass | 0.753s |
| Line 23: type error binary op.invalid | ✅ pass | 0.753s |

#### 05-shapes (3 tests, 0.080s)

##### shapes.pest

| Test | Outcome | Time |
|------|---------|-----:|
| It states the shape of a value once, for the run and for the analyser | ✅ pass | 0.003s |
| It names where a value stops fitting | ✅ pass | 0.002s |
| Draws data from the same type | ✅ pass | 0.075s |

#### 04-architecture (4 tests, 0.019s)

##### rules.pest

| Test | Outcome | Time |
|------|---------|-----:|
| Every event object declares strict types | ✅ pass | 0.004s |
| The impact tier does not reach the browser tier | ✅ pass | 0.004s |
| The retrigger endpoint stays inside the watch tier | ✅ pass | 0.006s |
| Impact value objects are immutable | ✅ pass | 0.004s |

#### 02-pest-dialect (16 tests, 0.017s)

##### basics.pest

| Test | Outcome | Time |
|------|---------|-----:|
| A test is a description and a closure | ✅ pass | 0.003s |
| It rounds up | ✅ pass | 0.001s |
| Expectations > it chains | ✅ pass | 0.001s |
| Expectations > it negates with not | ✅ pass | 0.001s |
| Expectations > it reaches into values with higher-order expectations | ✅ pass | 0.001s |
| Hooks > it sees the value the hook set | ✅ pass | 0.001s |
| Hooks > it sees it again, freshly | ✅ pass | 0.001s |
| It uppercases with data set "lowercase" | ✅ pass | 0.001s |
| It uppercases with data set "mixed" | ✅ pass | 0.001s |
| It uppercases with data set "already" | ✅ pass | 0.001s |
| It adds any two positives with data set "0 / 0" | ✅ pass | 0.001s |
| It adds any two positives with data set "0 / 1" | ✅ pass | 0.001s |
| It adds any two positives with data set "1 / 0" | ✅ pass | 0.001s |
| It adds any two positives with data set "1 / 1" | ✅ pass | 0.001s |
| It fails on purpose | ✅ pass | 0.001s |
| It belongs to a group | ✅ pass | 0.001s |

#### 03-doubles (4 tests, 0.006s)

##### Payments

| Test | Outcome | Time |
|------|---------|-----:|
| A stub answers without being verified | ✅ pass | 0.003s |
| A mock verifies how it was called | ✅ pass | 0.001s |
| Unconfigured methods return usable defaults | ✅ pass | 0.001s |
| Consecutive calls can differentiate | ✅ pass | 0.001s |

#### 01-phpunit-dialect (6 tests, 0.004s)

##### Calculator

| Test | Outcome | Time |
|------|---------|-----:|
| Adds two numbers | ✅ pass | 0.002s |
| Sums a list with data set "empty" | ✅ pass | 0.001s |
| Sums a list with data set "one item" | ✅ pass | 0.000s |
| Sums a list with data set "several" | ✅ pass | 0.000s |
| Multiplies | ✅ pass | 0.000s |
| Uses the product of its dependency | ✅ pass | 0.000s |

#### 06-equivalent-mutants (2 tests, 0.002s)

##### Inventory

| Test | Outcome | Time |
|------|---------|-----:|
| First is the first item or null | ✅ pass | 0.002s |
| Restock returns the count | ✅ pass | 0.001s |

#### src (0.002s)

#### Test (2 tests, 0.001s)

##### TestId

| Test | Outcome | Time |
|------|---------|-----:|
| Test id::from string with data set "crucible 1" | ✅ pass | 0.001s |
| Test id::from string with data set "crucible 2" | ✅ pass | 0.000s |

#### Reporting (2 tests, 0.001s)

##### PrettyName

| Test | Outcome | Time |
|------|---------|-----:|
| Pretty name::of file with data set "check 1" | ✅ pass | 0.000s |
| Pretty name::of file with data set "a file just called Test keeps its name" | ✅ pass | 0.000s |

