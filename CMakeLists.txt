#
# valijson
#
fips_begin_lib(valijson)
    fips_dir(include/compat)
    fips_files(
        optional.hpp
    )

    fips_dir(include/valijson)
    fips_files(
        constraint_builder.hpp
        schema.hpp schema_parser.hpp
        subschema.hpp validation_results.hpp
        validation_visitor.hpp validator.hpp
    )

    fips_dir(include/valijson/adapters)
    fips_files(
        adapter.hpp basic_adapter.hpp
        frozen_value.hpp json11_adapter.hpp
        jsoncpp_adapter.hpp nlohmann_json_adapter.hpp
        picojson_adapter.hpp property_tree_adapter.hpp
        rapidjson_adapter.hpp
    )

    fips_dir(include/valijson/constraints)
    fips_files(
        basic_constraint.hpp concrete_constraints.hpp
        constraint.hpp constraint_visitor.hpp
    )

    fips_dir(include/valijson/internal)
    fips_files(
        custom_allocator.hpp json_pointer.hpp
        json_reference.hpp uri.hpp
    )

    fips_dir(include/valijson/utils)
    fips_files(
        file_utils.hpp json11_utils.hpp jsoncpp_utils.hpp
        nlohmann_json_utils.hpp picojson_utils.hpp
        property_tree_utils.hpp rapidjson_utils.hpp
        utf8_utils.hpp
    )

    fips_dir(thirdparty/json11-2016-01-26)
    fips_files(json11.hpp json11.cpp)

fips_end_lib(zlib)
