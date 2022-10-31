package(default_visibility = ["PUBLIC"])

go_module(
    name = "elastic_go-elasticsearch_v8",
    hashes = ["9c12b0f33abacded3946a6f2df19a0d786d9b55c18eeeec144b0f83d3a67964d"],
    install = [
        ".",
        "esapi",
        "internal/version",
    ],
    module = "github.com/elastic/go-elasticsearch/v8",
    version = "v8.3.0",
    deps = [
        ":elastic-transport_v8",
    ],
)

go_module(
    name = "elastic-transport_v8",
    hashes = ["87f5da003fa8c636f760287252103fe6bc013bbe36b1de5742bbd5a5dc8c4b82"],
    install = [
        "elastictransport",
        "elastictransport/version",
    ],
    module = "github.com/elastic/elastic-transport-go/v8",
    version = "v8.1.0",
)

go_module(
    name = "go-jira",
    hashes = ["af8883e5c9ac1fbfd07727e6781f935d586b7f6d9c502543c711e9458f20955d"],
    licences = ["MIT"],
    module = "github.com/andygrunwald/go-jira",
    version = "v1.12.0",
    deps = [
        ":go-querystring",
        ":jwt-go",
        ":pkg_errors",
        ":structs",
        ":tgo",
    ],
)

go_module(
    name = "go-querystring",
    hashes = ["c26c807bcb6fd54bda31e3c5030902b74665348224d4b67968f0347e7dac263f"],
    install = ["query"],
    licences = [
        "BSD-3-Clause",
    ],
    module = "github.com/google/go-querystring",
    version = "v1.0.0",
)

go_module(
    name = "jwt-go",
    hashes = ["f91120578568670187c28da4f6150f5b273608374a3fc0c8f98c83a015943dea"],
    licences = ["mit"],
    module = "github.com/dgrijalva/jwt-go",
    version = "v3.2.0+incompatible",
)

go_module(
    name = "structs",
    hashes = ["0474e169b599f90948628bdf9e2cce4d2edf449cfabc6db812b786220ac7df46"],
    licences = ["mit"],
    module = "github.com/fatih/structs",
    version = "v1.1.0",
)

go_module(
    name = "tgo",
    hashes = ["89a7ec75f93693dd8166178021dfb3e385ded8d8615e6c119c27231e0c4f1c94"],
    install = [
        "tcontainer",
        "treflect",
    ],
    licences = ["BSD 3-Clause"],
    module = "github.com/trivago/tgo",
    version = "v1.0.7",
)

go_module(
    name = "gogo_protobuf",
    hashes = ["ae0cd2f97d32d13742215b47db463bfaa6df772b6ae808f1ea53c1dc190e9304"],
    install = [
        "gogoproto",
        "proto",
        "sortkeys",
    ],
    module = "github.com/gogo/protobuf",
    version = "v1.3.2",
)

go_module(
    name = "protobuf",
    download = ":protobuf_download",
    hashes = ["a7248005f1f893498d86d4823f9ce1bd50bc40078fcbc2fffcdc7232ab835f2a"],
    install = [
        "proto",
        "ptypes",
        "ptypes/any",
        "ptypes/duration",
        "ptypes/timestamp",
        "jsonpb",
    ],
    module = "github.com/golang/protobuf",
    strip = [
        "proto/proto3_proto",
        "conformance",
    ],
)

go_mod_download(
    name = "protobuf_download",
    hashes = ["ca0fd0012898cb4d62d3def045e3ff1825d0236f9bf7240ca53afb401831fc84"],
    module = "github.com/golang/protobuf",
    version = "v1.3.2",
)

go_module(
    name = "protoc-gen-go",
    binary = True,
    download = ":protobuf_download",
    hashes = ["9c0a6d6312dc36e23d8738d2d15d0dfa06cb996ab7f45e0d124cb6d65fbdb40f"],
    install = ["protoc-gen-go"],
    module = "github.com/golang/protobuf",
    deps = [":protobuf"],
)

go_module(
    name = "google_uuid",
    hashes = ["06b171f08cecd8e709716212dbbdcf1a710dc6a5c608f4e17d57c7e06d3f338a"],
    module = "github.com/google/uuid",
    version = "v1.1.1",
)

go_module(
    name = "mitchellh_go-homedir",
    hashes = ["5683dafd077dee1797f5b7de35b6926f1e58594e7346684c7f8d27ee2326d8f5"],
    module = "github.com/mitchellh/go-homedir",
    version = "v1.1.0",
)

go_module(
    name = "speps_go-hashids",
    hashes = ["add2109790b506b109a5af5cddc913cde3ff841f4d92d414bfac77ee6aeb32b0"],
    module = "github.com/speps/go-hashids",
    version = "v2.0.0",
)

go_module(
    name = "spf13_cobra",
    hashes = ["47234725071412af1e3f3ef3a904428bb5c772a8f634610cde0df74354919b15"],
    licences = ["apache-2.0"],
    module = "github.com/spf13/cobra",
    version = "v0.0.5",
    deps = [
        ":spf13_pflag",
    ],
)

go_module(
    name = "spf13_viper",
    hashes = ["43f5cea8955c975ba983c32137608c30e73840dde5e1f04e8f16a2289f966d01"],
    licences = ["mit"],
    module = "github.com/spf13/viper",
    version = "v1.7.1",
    deps = [
        ":fsnotify",
        ":hashicorp_hcl",
        ":ini_v1",
        ":magiconair_properties",
        ":mitchellh_mapstructure",
        ":pelletier_go-toml",
        ":spf13_afero",
        ":spf13_cast",
        ":spf13_jwalterweatherman",
        ":spf13_pflag",
        ":subosit_gotenv",
        ":yaml.v2",
    ],
)

go_module(
    name = "subosit_gotenv",
    hashes = ["a35f690f4798ec6d35a7a759b68136e96e254d07ba4efe8b0fa0e2ee0a1a7984"],
    licences = ["MIT"],
    module = "github.com/subosito/gotenv",
    version = "v1.2.0",
)

go_module(
    name = "ini_v1",
    hashes = ["fc9fc8984b664eebd71b2374a1093e2914dc6ab01ce6d170332af9cae1d91c94"],
    licences = ["Apache-2.0"],
    module = "gopkg.in/ini.v1",
    version = "v1.62.0",
)

go_module(
    name = "stretchr_testify",
    hashes = ["5b0e5560714d63c92fde0c5d7ee2b276310460e2f34d20df64b6cf72a39fc528"],
    install = [
        "assert",
        "mock",
        "require",
    ],
    module = "github.com/stretchr/testify",
    version = "v1.7.0",
    deps = [
        ":davecgh_go-spew",
        ":pmezard_go-difflib",
        ":stretchr_objx",
        ":yaml_v3",
    ],
)

go_module(
    name = "yaml_v3",
    hashes = ["4b8d78e7e61d57164475aec8d579e227a36bc71bd911d9fef1e3957d06632404"],
    licences = ["Apache-2.0"],
    module = "gopkg.in/yaml.v3",
    version = "496545a6307b2a7d7a710fd516e5e16e8ab62dbc",
)

go_module(
    name = "davecgh_go-spew",
    hashes = ["dba04cbc599861e2ed3f086ed75471b009ddd8f90677be3e181c9ee35a99cb47"],
    install = [
        "spew",
    ],
    module = "github.com/davecgh/go-spew",
    version = "v1.1.1",
)

go_module(
    name = "pmezard_go-difflib",
    hashes = ["3d6ad64cae5e8c10ce29f343f296f36e79a352e7408d8bbb580df11d3bb86c44"],
    install = [
        "difflib",
    ],
    module = "github.com/pmezard/go-difflib",
    version = "v1.0.0",
)

go_module(
    name = "stretchr_objx",
    hashes = ["2c28eb6b522077a0b755be3d52c526e656c19242b7b6ffa6f2c3ad3199d0e4ee"],
    module = "github.com/stretchr/objx",
    version = "v0.1.1",
)

go_module(
    name = "fsnotify",
    hashes = ["b4f4fed70aed910400abd778ca142124ab57016965815f9e765a9dfa826a4554"],
    module = "github.com/fsnotify/fsnotify",
    version = "v1.4.7",
    deps = [
        ":x_sys",
    ],
)

go_module(
    name = "x_sys",
    hashes = ["35f2e3017064bd104e476c17098916405b9f8c4a3e4321472847d324f11427fb"],
    install = [
        "unix",
        "cpu",
    ],
    module = "golang.org/x/sys",
    version = "v0.1.0",
)

go_module(
    name = "hashicorp_hcl",
    hashes = ["86a678f1718aef0b0b2b7e636c3247218349eddf9471efc94ce7ab5eec8676a8"],
    install = [
        ".",
        "...",
    ],
    module = "github.com/hashicorp/hcl",
    version = "v1.0.0",
)

go_module(
    name = "magiconair_properties",
    hashes = ["6171853e4e297fcb4c0e387fb1e10375b0df48ee1a09f1fa448b6e5e8ccb1281"],
    module = "github.com/magiconair/properties",
    version = "v1.8.0",
)

go_module(
    name = "mitchellh_mapstructure",
    hashes = ["70ea1f13980d5fa7af8d99c96899e46f716cfa8db49b6718aa12af66d6c06385"],
    module = "github.com/mitchellh/mapstructure",
    version = "v1.1.2",
)

go_module(
    name = "pelletier_go-toml",
    hashes = ["8576ca8e0da2d9a5727e3dcae61f4f06b59a900b8f310fb3cde1d022552fba6d"],
    module = "github.com/pelletier/go-toml",
    version = "v1.2.0",
)

go_module(
    name = "spf13_cast",
    hashes = ["49b937dd91e401db32cc81b1b17f6ef140dfad83bf72bd4c508ead48fdbbf39c"],
    module = "github.com/spf13/cast",
    version = "v1.3.0",
)

go_module(
    name = "spf13_jwalterweatherman",
    hashes = ["190f2728886856723bf25040daa8decba2e5e3a5ef7a118c891db2ee7a016912"],
    module = "github.com/spf13/jwalterweatherman",
    version = "v1.0.0",
)

go_module(
    name = "yaml.v2",
    hashes = ["431a83405c7f428d4c8b5a8adfef6aba0d9a37670afd683fb46c14cbcb32d15c"],
    module = "gopkg.in/yaml.v2",
    version = "v2.2.2",
)

go_module(
    name = "spf13_afero",
    hashes = ["3797020031356c63f776784d4afa2cd9838c523fb24ef29577f9d85732b14ecf"],
    install = [
        ".",
        "mem",
    ],
    module = "github.com/spf13/afero",
    version = "v1.1.2",
    deps = [
        ":x_text",
    ],
)

go_module(
    name = "x_text",
    hashes = ["a4f1f3a38089f4c13693d96c542182d4b9395b029ef4c5bd6a19e8cf7fda7fbb"],
    install = [
        "encoding",
        "encoding/...",
        "transform",
        "unicode/...",
        "secure/bidirule",
    ],
    module = "golang.org/x/text",
    version = "v0.3.0",
)

go_module(
    name = "spf13_pflag",
    hashes = ["fafd4358ff6970a1e578267eee936582c3b5f1c5b306407cb9e2aa4dcbd07d6f"],
    module = "github.com/spf13/pflag",
    version = "v1.0.3",
)

go_module(
    name = "pkg_errors",
    hashes = ["791eb672b2448c3a012370add6e2c07a9ccb57f1844419c572bfa7b93432967d"],
    module = "github.com/pkg/errors",
    version = "v0.8.1",
)

go_module(
    name = "evanphx_json-patch",
    hashes = ["9574f9eb929dcb0276943ac961939de7619e777381fd00fd4391b6175d207ac7"],
    module = "github.com/evanphx/json-patch",
    version = "v4.5.0",
    deps = [
        ":pkg_errors",
    ],
)

go_module(
    name = "ghodss_yaml",
    hashes = ["29db4b0ee39b89bcf365ccc80d167c799f776d264157aef90ef920e89df59ed8"],
    module = "github.com/ghodss/yaml",
    version = "v1.0.0",
    deps = [
        ":yaml.v2",
    ],
)

KUBERNETES_VERSION = "1.19.11"

go_module(
    name = "apimachinery",
    hashes = ["7602f9266dd785c0dc848c2b40df14065220ccc2d2f64c5afd5fa28f020dd275"],
    install = [
        "pkg/apis/meta/v1",
        "pkg/runtime/schema",
        "pkg/api/resource",
        "pkg/conversion",
        "pkg/labels",
        "pkg/runtime",
        "pkg/util/intstr",
        "pkg/util/runtime",
        "pkg/util/sets",
        "pkg/util/validation",
        "pkg/util/json",
        "pkg/util/errors",
        "pkg/util/naming",
        "pkg/util/net",
        "pkg/util/validation/...",
        "pkg/fields",
        "pkg/conversion/...",
        "pkg/watch",
        "pkg/types",
        "pkg/selection",
        "third_party/forked/golang/reflect",
    ],
    module = "k8s.io/apimachinery",
    strip = [
        "pkg/util/proxy",
        "pkg/util/jsonmergepatch",
        "pkg/runtime/serializer/recognizer/testing",
    ],
    version = "kubernetes-%s" % KUBERNETES_VERSION,
    deps = [
        ":gogo_protobuf",
        ":google_gofuzz",
        ":inf.v0",
        ":klog",
        ":structured_merge_diff",
        ":x_net",
    ],
)

go_module(
    name = "structured_merge_diff",
    hashes = ["d32554e42cc7ad537545862c448477f23ef869a4b56c021b67a9d0abd343a87e"],
    install = [
        "value",
    ],
    module = "sigs.k8s.io/structured-merge-diff/v4",
    version = "v4.2.3",
    deps = [
        ":json_iterator",
        ":yaml.v2",
    ],
)

go_module(
    name = "json_iterator",
    hashes = ["8d207d75bac890386a84e73ed05b428eec5d895c2ea8631fa086ff80ec3a22db"],
    module = "github.com/json-iterator/go",
    version = "v1.1.12",
    deps = [
        ":modern_go",
        ":modern_go_concurrent",
    ],
)

go_module(
    name = "modern_go",
    hashes = ["4685241918d6bc5985b0bed975c0b4f5eb1556122409c6e261d0f57091dcaa81"],
    module = "github.com/modern-go/reflect2",
    version = "v1.0.2",
)

go_module(
    name = "modern_go_concurrent",
    hashes = ["810908664f8b0073fcc52d8771586936d53bf4f5bff99e5760a2b7d46b2423e0"],
    module = "github.com/modern-go/concurrent",
    version = "1.0.3",
)

go_module(
    name = "google_gofuzz",
    hashes = ["3c1415b49842a84af07d85695ac04c205ef4a5cf57b9f1e202550319aaa07d57"],
    module = "github.com/google/gofuzz",
    version = "v1.0.0",
)

go_module(
    name = "inf.v0",
    hashes = ["8a1234d6fa309c8b3b5ea5353adac45797e19b8836a0ba21718d068f871a618c"],
    module = "gopkg.in/inf.v0",
    version = "v0.9.1",
)

go_module(
    name = "x_net",
    hashes = ["b6ef1592124d27012157c4dbcb0d0d6c5b43bf942fb67eec6a0d9f01fbbc28a6"],
    install = ["..."],
    module = "golang.org/x/net",
    strip = [
        "http2/h2demo",
        "http2/h2i",
    ],
    version = "v0.1.0",
    deps = [
        ":x_sys",
        ":x_text",
    ],
)

go_module(
    name = "klog",
    hashes = ["65611c0c524fd566317544401200a461343706cf72c35981a7179c63a3f47e3f"],
    install = [
        "internal/buffer",
        "internal/clock",
        "internal/dbg",
        "internal/serialize",
        "internal/severity",
        "",
    ],
    module = "k8s.io/klog/v2",
    version = "v2.80.1",
    deps = [":logr"],
)

go_module(
    name = "logr",
    hashes = ["b670a256ceea9b44c27cd4e98d95dfc23aa27a0e08b0a29a2d22a62eead34d5c"],
    module = "github.com/go-logr/logr",
    version = "v1.2.3",
)

go_module(
    name = "golang-migrate_migrate",
    hashes = ["dd77862a453e8e753f298f6503da12ef9bb534f3a1fab9df9c6e43f39e9cffb3"],
    install = [
        ".",
        "database/postgres",
        "source/go_bindata",
        "database",
        "internal/...",
        "source",
    ],
    module = "github.com/golang-migrate/migrate/v4",
    version = "v4.7.0",
    deps = [
        ":hashicorp_go-multierror",
        ":lib_pq",
    ],
)

go_module(
    name = "hashicorp_go-multierror",
    hashes = ["98baeb95328c101e7ea45a7aa91c085722ac85bbfd8061cac56870961c9d2d0e"],
    module = "github.com/hashicorp/go-multierror",
    version = "v1.0.0",
    deps = [
        ":hashicorp_errwrap",
    ],
)

go_module(
    name = "hashicorp_errwrap",
    hashes = ["60ee2450615b430918e85a89aae9ff8cb0310ff9e6eed00ce4f9e0be20bb4032"],
    module = "github.com/hashicorp/errwrap",
    version = "v1.0.0",
)

go_module(
    name = "lib_pq",
    hashes = ["8fd2b25ed50efa405fc127081cac8d9c272d02a8d941a22a0c28524095569a2d"],
    install = [
        ".",
        "oid",
        "scram",
    ],
    module = "github.com/lib/pq",
    version = "v1.10.3",
)

go_module(
    name = "jmoiron_sqlx",
    hashes = ["9ddc949567c804ecdc00addd8c8c9f69c7f43f4907a8a743c14a5e59ca81b814"],
    install = [
        ".",
        "...",
    ],
    module = "github.com/jmoiron/sqlx",
    version = "v1.2.0",
)

go_mod_download(
    name = "mockgen_download",
    hashes = ["62c71cc09d45f5fb2b2a64a877a99b333295af4425918a655c2df8c1eac7879b"],
    module = "github.com/golang/mock",
    version = "v1.4.4",
)

go_module(
    name = "mockgen",
    binary = True,
    download = ":mockgen_download",
    hashes = ["b1d226ce7c379454d7cabc008d6dc4e15da1aa004bc34ff79dea01dec7dabba6"],
    install = ["mockgen"],
    licences = ["apache-2.0"],
    module = "github.com/golang/mock",
    deps = [":x_tools"],
)

go_module(
    name = "mock",
    download = ":mockgen_download",
    hashes = ["9c0a6d6312dc36e23d8738d2d15d0dfa06cb996ab7f45e0d124cb6d65fbdb40f"],
    install = ["..."],
    licences = ["apache-2.0"],
    module = "github.com/golang/mock",
    deps = [
        ":x_tools",
    ],
)

go_module(
    name = "h2non_parth",
    hashes = ["4e5c8f9ba9491ae57321ea39d80b42305999bd7ba998eb316f9c767a69d5ef81"],
    licences = ["MIT"],
    module = "github.com/h2non/parth",
    version = "v0.0.0-20190131123155-b4df798d6542",
)

go_module(
    name = "h2non_gentleman",
    hashes = ["c2e27a83edd1b061e5759d7a0fcc3ddcb04a520e6ebe2c649de0a76cc123ecfb"],
    install = ["..."],
    licences = ["MIT"],
    module = "gopkg.in/h2non/gentleman.v1",
    strip = ["_examples"],
    version = "v1.0.4",
    deps = [
        ":x_net",
    ],
)

go_module(
    name = "h2non_gock",
    hashes = ["8d037bdc6da1575efc19094b1acffbffeda2ef0b58c3af0f57dff65297ef5b17"],
    licences = ["MIT"],
    module = "gopkg.in/h2non/gock.v1",
    version = "v1.0.16",
    deps = [
        ":h2non_gentleman",
        ":h2non_parth",
        ":x_net",
    ],
)

go_module(
    name = "x_tools",
    hashes = ["94defd9a747852d72eacc8fc95e3be06b433faed357649019ecd1dcbf14a89c1"],
    install = [
        "cover",
        "present",
        "go/packages",
        "go/internal/packagesdriver",
        "internal/gocommand",
        "internal/packagesinternal",
        "go/gcexportdata",
        "go/internal/gcimporter",
        "go/ast/astutil",
    ],
    licences = ["bsd-3-clause"],
    module = "golang.org/x/tools",
    version = "5bcca83a78812bd91ce8cb29be4fc4521cdc8f6f",
    deps = [
        ":x_errors",
        ":x_mod",
    ],
)

go_module(
    name = "x_crypto",
    hashes = ["822ba7c1ffa310e6363b79f1a4e32af144a201cf0948e02d56c5f8bab6bec271"],
    install = ["..."],
    licences = ["bsd-3-clause"],
    module = "golang.org/x/crypto",
    strip = ["acme/autocert"],
    version = "123391ffb6de907695e1066dc40c1ff09322aeb6",
    deps = [":x_sys"],
)

go_module(
    name = "x_errors",
    hashes = ["6cd513303dcebeaf24fe0413da89ff0b8489554749fa23425e9149fc377cc327"],
    install = [
        ".",
        "...",
    ],
    licences = ["bsd-3-clause"],
    module = "golang.org/x/xerrors",
    version = "a5947ffaace3e882f334c1750858b4a6a7e52422",
    deps = [":x_sys"],
)

go_module(
    name = "x_mod",
    hashes = ["45e3c27276f4eed7431ecafd4a30ba6dd6aa507ba87f3423c6ad13eecd481e63"],
    install = [
        "semver",
        "module",
    ],
    licences = ["bsd-3-clause"],
    module = "golang.org/x/mod",
    version = "v0.4.2",
    deps = [":x_errors"],
)

go_module(
    name = "x_sync",
    hashes = ["af9bc4b4f7673e72d4f6604c46eff1c22b54fea400717d1f99777a072e0c24c3"],
    install = ["..."],
    licences = ["bsd-3-clause"],
    module = "golang.org/x/sync",
    version = "fd80eb99c8f653c847d294a001bdf2a3a6f768f5",
    deps = [
        ":x_net",
    ],
)

go_module(
    name = "aws-sdk-go-v2-securityhub",
    hashes = ["7865ce25d13af06484bb1eaf3f9b7db1e1e04b0b3d9e7b377f6d4268e4d5b9e0"],
    install = ["types"],
    licences = ["Apache License 2.0"],
    module = "github.com/aws/aws-sdk-go-v2/service/securityhub",
    version = "v1.21.2",
    deps = [
        ":smithy-go",
    ],
)

go_module(
    name = "smithy-go",
    hashes = ["bd52176ea9ff58a4809af02058fc3530645cc953381975377356b173a8024605"],
    install = ["..."],
    licences = ["Apache License 2.0"],
    module = "github.com/aws/smithy-go",
    version = "v1.11.2",
    deps = [":go-cmp"],
)

go_module(
    name = "go-cmp",
    hashes = ["c0fafa9d7793a4daec5d1f056ed2bfff29a903149002324968f94aa9be4c2492"],
    install = ["..."],
    licences = ["BSD-3-Clause"],
    module = "github.com/google/go-cmp",
    version = "v0.5.8",
)

go_module(
    name = "go-sarif",
    hashes = ["f028d247cd9763396fe64cbaa401394429502dc7887aef776bd2cfdfc9f3c8ef"],
    install = ["..."],
    licences = ["Unlicense license"],
    module = "github.com/owenrumney/go-sarif/v2",
    version = "v2.1.2",
)
