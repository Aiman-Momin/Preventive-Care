PreventiveCare Module

A simple Move module to manage micro-payments for preventive healthcare services on the Aptos blockchain.

Features
Patient Setup: Patients can create a care account with an initial deposit and a linked provider.
Authorized Payments: Only the assigned healthcare provider can process payments.
Care Tracking: Automatically records the timestamp of the last checkup.

Functions
setup_care_account(patient: &signer, provider: address, initial_deposit: u64)
Initializes a care account for a patient with a deposit and assigned provider.
process_care_payment(provider: &signer, patient_address: address, service_cost: u64)
Allows the authorized provider to deduct service cost from the patient’s care account.

