# showing-the-Step-Definition-for-verifying-for-a-specific-name-or-text-to-be-present-
@then('I should see "{text}" on the page')
def step_impl(context, text):
    assert text in context.browser.page_source
