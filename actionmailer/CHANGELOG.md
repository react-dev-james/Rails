## Rails 5.2.0.beta2 (November 28, 2017) ##

*   No changes.


## Rails 5.2.0.beta1 (November 27, 2017) ##

*   Add `assert_enqueued_email_with` test helper.

        assert_enqueued_email_with ContactMailer, :welcome do
          ContactMailer.welcome.deliver_later
        end

    *Mikkel Malmberg*

*   Allow Action Mailer classes to configure their delivery job.

        class MyMailer < ApplicationMailer
          self.delivery_job = MyCustomDeliveryJob

          ...
        end

    *Matthew Mongeau*



